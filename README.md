## Neuron ESB Plugin for New Relic

[![Build status](https://ci.appveyor.com/api/projects/status/j9r0spoh9w62jc9m?svg=true)](https://ci.appveyor.com/project/brentpabst/newrelic-neuronesb-plugin)
[![Coverage Status](https://coveralls.io/repos/github/203sol/newrelic-neuronesb-plugin/badge.svg?branch=master)](https://coveralls.io/github/203sol/newrelic-neuronesb-plugin?branch=master)
[![Stories in Backlog](https://badge.waffle.io/203sol/newrelic-neuronesb-plugin.svg?label=backlog&title=Backlog)](http://waffle.io/203sol/newrelic-neuronesb-plugin)
[![Gitter](https://badges.gitter.im/203sol/newrelic-neuronesb-plugin.svg)](https://gitter.im/203sol/newrelic-neuronesb-plugin?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

Prerequisites
-------------
- A New Relic account. Signup for a free account at [http://newrelic.com](http://newrelic.com)
- A server running Neudesic's Neuron 3.5 or greater. Download the latest versions of Neuron [here](http://www.neuronesb.com/product/download).
- .NET 3.5 on Windows Server.

Installation
-------------

The Neuron ESB plugin can be [installed manually](#running-the-agent) or automatically with the [New Relic Platform Installer](#npi).

Additional information on New Relic's Platform install can be found in their [documentation](https://discuss.newrelic.com/t/getting-started-with-the-platform-installer/842).

Running the Agent
-----------------

#### <a name="npi">Option 1: New Relic Platform Installer</a>

1. Install the NPI tool, if not done already.
2. Install the Plugin: `npi install com.203sol.newrelic.neuronesb`
3. Make any necessary changes to `plugin.json` and `newrelic.json` in the `<plugindir>/config` directory.


#### <a name="running-the-agent">Option 2: Manual Installer - Option 1 is far easier!</a>

1. No seriously, Option 1 is easier.
2. Doanload the latest `com.203sol.newrelic.neuronesb.Z.Y.Z.zip` from the [GitHub releases page](https://github.com/203sol/newrelic-neuronesb-plugin/releases).
3. Extract the downloaded archive to the location you want to run the Neuron ESB plugin from
4. Copy `<plugindir>/config/newrelic.template.json` to `<plugindir>/config/newrelic.json`
5. Copy `<plugindir>/config/plugin.template.json` to `<plugindir>/config/plugin.json`
6. Update `<plugindir>/config/newrelic.json` with your New Relic license key.
7. Update `<plugindir>/config/plugin.json` to make any required changes.
8. From CMD or PowerShell run:+1: `./plugin.exe`
9. Wait a few minutes for New Relic to begin processing the data sent from your agent.
10. Log into your New Relic account at [http://newrelic.com](http://newrelic.com) and click on `Neuron ESB` from the Plugin page to view your metrics.

Source Code
-----------

This plugin can be found at [https://github.com/203sol/newrelic-neuronesb-plugin/](https://github.com/203sol/newrelic-neuronesb-plugin/)

Contributing
-----------

Feel free to fork us, submit issues, and pull requests!
