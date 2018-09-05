# Botpress-kick-starter

This is a example bot that is integrated with Rocket.Chat.

We used the command `botpress init` and followed the steps in the `##instalation`
topic to build this bot, so you can easily run `botpress start` to see the 
**botpress bot** working in Rocket.Chat.

This bot is using version `10.34.0` of **botpress**.

## Overview

![botpress-rocketchat](https://github.com/RocketChat/botpress-channel-rocketchat/wiki/images/botpress.gif)

### Create you own bot

* Install botpress:

```sh
npm install -g botpress@10.34.0
```

* Create your bot:

```sh
mkdir bot
cd bot
botpress init
```

* After add your bot data install the dependencies:

```sh
npm install

npm install botpress-channel-rocketchat
```

* Create the file `config/channel-rocketchat.json` and insert your bot data:

```json
{
    "ROCKETCHAT_USER": "botpress",
    "ROCKETCHAT_PASSWORD": "botpress",
    "ROCKETCHAT_URL": "http://localhost:3001",
    "ROCKETCHAT_USE_SSL": "false",
    "ROCKETCHAT_ROOM": "GENERAL",
    "scope": ""
}
```

* Run your bot:

```sh
botpress start
```

### Using this example bot 

* Install your bot dependencies:

```sh
npm install
```

* Update the file `config/channel-rocketchat.json` and insert your bot data:

```json
{
    "ROCKETCHAT_USER": "botpress",
    "ROCKETCHAT_PASSWORD": "botpress",
    "ROCKETCHAT_URL": "http://localhost:3001",
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

* To access the botpress instance go to `localhost:3000` (you can change this configuration at `botfile.js`)

### Livechat

If you want to use your botpress bot in a LiveChat, follow this steps:

* The Livechat allows a feature of a window that can be integrated to other pages. To activate it, you must access again the **Administration** option, by clicking on three points icon, on the left side menu. Then click on **Livechat** option.

* On the next screen, mark the **Livechat enabled** option as True, and the **Show pre-registration form** option as False, in order to not be asked for email and password when using chat. Click then in **SAVE CHANGES**.

* Close the left side menu, and click on three points icon. Select the **Livechat** option.

* At the right side menu, select the **User Management** option. You must add the bot as an agent, so search for botnat, then click in **ADD**.

* Now it is necessary to create an department. On the left side menu, click on **Departments**, and then click in **NEW DEPARTMENT**.

* On the next screen, write a name and a description for the department and add the bot by selecting him on **Available agents**. Then click on **Save** option.

* On the left side menu, click at **Installation**. Now you only need to copy and paste the code on your site, where you want to integrate the conversation window.

* After integrating the code to your site, a window like the one showed in the image should be available, and ready to use.

### Deploy

Check [Heroku](https://botpress.io/docs/deploy/heroku/) and [AWS](https://botpress.io/docs/deploy/aws/) deploy tutorials to get started

### Development

To learn more on how to work with [Botpress](https://botpress.io/) you can read [here](https://botpress.io/docs/getting_started/).
