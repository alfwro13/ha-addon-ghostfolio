# Home Assistant App: Ghostfolio

Manage your wealth like a boss.

## About

[Ghostfolio][ghostfolio] is a privacy-first, open source dashboard for your personal finances.
Break down your asset allocation, know your net worth and make solid, data-driven investment decisions.

This app allows you to run [Ghostfolio][ghostfolio] on your Home Assistant server based on the the official Ghostfolio [docker image][docker].

![Ghostfolio Version][ghostfolio-version]
![Supported Architectures][archs]

| Light Mode                 | Dark Mode                |
| -------------------------- | ------------------------ |
| ![Light screenshot][light] | ![Dark screenshot][dark] |

## Requirements

Ghostfolio needs a PostgreSQL database.
I recommend using the [PostgreSQL App][alexbelgium-postgres] from @alexbelgium's repository if you aren't already using Postgres.

## Installation

The installation of this App is pretty straightforward and no different to installing any other Home Assistant app.

1. Add my [app repository][addons-repo] to Home Assistant or click the button below to open my app repository on your Home Assistant instance.

   [![Open add-on repo on your Home Assistant instance][repo-btn]][addon]

1. Install this app.
1. Install the PostgreSQL app and configure and start it, if you wish to use this app.
1. Enter your PostgreSQL configuration information.
1. Click the `Save` button to store your configuration.
1. Start the app.
1. Check the logs of the app to see if everything went well.
1. Click the `OPEN WEB UI` button to open Ghostfolio.

To monitor your Ghostfolio portfolio performance directly within Home Assistant, use the companion [Ghostfolio Home Assistant Integration](https://github.com/alfwro13/ghostfolio_ha_integration).

## Acknowledgments
This addon is maintained by @alfwro13.
Originally based on the [https://github.com/lildude/ha-addon-ghostfolio](https://github.com/lildude/ha-addon-ghostfolio). 


[addon]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Falfwro13%2Fha-addon-ghostfolio
[addons-repo]: https://github.com/alfwro13/ha-addon-ghostfolio
[alexbelgium-postgres]: https://github.com/alexbelgium/hassio-addons/tree/master/postgres
[archs]: https://img.shields.io/badge/dynamic/json?color=green&label=Arch&query=%24.arch&url=https%3A%2F%2Fraw.githubusercontent.com%2Falfwro13%2Fha-addon-ghostfolio%2Fmain%2Fconfig.json
[dark]: https://raw.githubusercontent.com/alfwro13/ha-addon-ghostfolio/main/imgs/screenshot-dark.png
[docker]: https://hub.docker.com/r/ghostfolio/ghostfolio
[ghostfolio-version]: https://img.shields.io/badge/dynamic/json?label=Ghostfolio%20Version&url=https%3A%2F%2Fraw.githubusercontent.com%2Falfwro13%2Fha-addon-ghostfolio%2Fmain%2Fbuild.json&query=%24.args.ghostfolio_version
[ghostfolio]: https://ghostfol.io
[light]: https://raw.githubusercontent.com/alfwro13/ha-addon-ghostfolio/main/imgs/screenshot-light.png
[postgres]: https://github.com/matt-FFFFFF/hassio-addon-postgres
[repo-btn]: https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg

