# Botpress-kick-starter

This is a example bot that is integrated with Rocket.Chat.

We used the command `botpress init` and followed the steps in the `##instalation`
topic to build this bot, so you can easily run `botpress start` to see the 
**botpress bot** working in Rocket.Chat.

## Overview

![botpress-rocketchat](https://github.com/RocketChat/botpress-channel-rocketchat/wiki/images/botpress.gif)

## Installation

* Install your bot dependencies:

```sh
npm install
```

* Update the file `config/channel-rocketchat.json` and insert yourt bot data:

```json
{
    "ROCKETCHAT_USER": "botpress",
    "ROCKETCHAT_PASSWORD": "botpress",
    "ROCKETCHAT_URL": "http://localhost:3000",
    "ROCKETCHAT_USE_SSL": "false",
    "ROCKETCHAT_ROOM": "GENERAL",
    "scope": ""
}
```

* Start your bot.

```sh
botpress start
```

* After that all your `dialogEngine` made in botpress flow will work, so send any
 message to the bot or the channels that you added it.

* To access the botpress instance go to `localhost:3001` (you can change this configuration at `botfile.js`)

## Troubleshooting

If the bot don't run, try to run:

```sh
npm audit fix
```

## Deploy

Check [Heroku](https://botpress.io/docs/deploy/heroku/) and [AWS](https://botpress.io/docs/deploy/aws/) deploy tutorials to get started

## Development

To learn more on how to work with [Botpress](https://botpress.io/) you can read [here](https://botpress.io/docs/getting_started/).
