# Botpress-kick-starter

This is a example bot that is integrated with Rocket.Chat.

## Overview

TODO

## Run bot

* Install all dependêncies:

`npm install`

* Up a instance of Rocket.chat with docker:

`docker-compose up mongo`
`docker-compose up rocketchat`

* Login and create the bot user at `http://localhost:3002`.

* Run the bot:

`botpress start` 

By default bot runs locally with web interface available at http://localhost:3000

After that all your `dialogEngine` made in botpress flow will work, so send any
 message to the bot or the channels that you added it.

## Deploy

Check [Heroku](https://botpress.io/docs/deploy/heroku/) and [AWS](https://botpress.io/docs/deploy/aws/) deploy tutorials to get started

## Development

To learn more on how to work with [Botpress](https://botpress.io/) you can read [here](https://botpress.io/docs/getting_started/).
