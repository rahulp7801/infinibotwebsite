---
description: >-
  These docs aim to help your understanding of InfiniBot and its features, as
  well as some basic info. NOTE: If you came here to access a commands list, you
  are in the wrong place. {Link to commands}
---

# Getting started

## Some things to set up for your server upon adding the bot

### Connect Last.fm

A popular service commonly used by avid music fans, Last.fm gives a detailed insight on your listening style. InfiniBot offers an integration between Discord and LastFM, so you can access your stats directly from the comfort of your Discord server. The command for setting it up is:

```text
#syntax
%fm set <username>
#example
%fm set babatunde
```

This command will save your LastFM information with InfiniBot, and you will only have to run it once.

#### The bot says my username is not valid?

This means that you incorrectly inputted your username into the bot. Go to [https://www.last.fm/](https://www.last.fm/) and look for your username by hovering over your profile picture in the top-right corner.

#### Why does it say I have no scrobbles?

This happens when your account is new, and you have not listened to anything recently. If that is not the case, patiently wait for a few minutes to see if the bot will update. If the problem still persists, contact the developers directly using the feedback command or join the support server.

#### The now playing command is showing the wrong track

More often than not, this is out of InfiniBot's control. This can mean one of two things:

1. You aren't listening to anything at the moment.
2. Your last.fm account has somehow been disconnected from your Spotify account. Try going to [https://www.last.fm/settings/applications](https://www.last.fm/settings/applications), disconnect "Spotify Scrobbling", wait for a few minutes, and then reconnect.

{% hint style="info" %}
InfiniBot is NOT affiliated with Last.fm or Spotify, so if you have any questions concerning scrobbling, please contact the former by visiting [https://www.last.fm/about/contact](https://www.last.fm/about/contact)
{% endhint %}

## Setting up the bot

### Welcomer

InfiniBot's welcoming system requires a one-time, easy, straightforward, and intuitive setup procedure. To begin, run the following command and its variants to start setup. The entire process should not be in excess of 5 minutes from start to finish.

```text
// get help on the command
%setup

// setup a specific aspect
%setup <aspect>

// setup everything
%setup all
```

#### If you run the "setup all" command

After this one-time, around 5 minute procedure, you can leave your server in the hands of InfiniBot! Its blazingly fast system will make sure that your server stays super clean! You will also notice that all of your preferences, such as the role you saved, your welcome message, all of that can be accessed by running the command shown below:

```text
%serverinfo
```

{% hint style="info" %}
Getting any errors during set up or is the bot unresponsive? Make sure the bot has the following permissions: 

**Embed Links, Attach Files, Read Messages, Send Messages, Manage Channels, and Manage Roles.**

Without all of these permissions, InfiniBot cannot moderate to its full extent!!!
{% endhint %}

#### What if I want to change some settings later?

All you have to do is run the "**setup**" command with the thing you would like to set up immediately after. If you aren't sure about which one you need, just run the **setup** command and it will bring up a help menu.

```text
// for a specific module
%setup <module>

// example
%setup welcomechannel

// for help
%setup
```

### Moderation

A main part of InfiniBot is its extensive tools for moderating a server. The main things you need to set up for moderation are **logging** and **ticketing.**

#### **Logging**

InfiniBot keeps track of all of the events in your server so you don't miss a thing. However, this is toggled off by default, and you need to either specify or let the bot create a log channel! This is simple, you can accomplish this by running the following command.

```text
%setup logging
```

This both toggles logging on and asks you for a channel you want the logs to be redirected to.

{% hint style="info" %}
If the bot is unresponsive \(worst-case scenario\), give the bot administrator permissions to see if that was the reason it was blocking.
{% endhint %}

#### Ticketing System

InfiniBot comes built-in with an advanced ticketing system. By default, all logs will be redirected to the logging channel that was specified as you were setting up logging, but this feature can be customized. To set this up, it is a one-time command as shown below: 

```text
%setupticketing
```

The way the ticketing system works for InfiniBot is the bot sends a message, and adds a reaction, that if the users click on it, they will open a ticket. So, the bot will initially prompt you to specify where this message should be sent. After that, it will ask you if you want it to ping a role when a ticket is created. After these two steps, the bot will send the message and your ticketing system is all set up!

{% hint style="info" %}
If an error arises, this most likely means the bot does not have adequate permissions to create channels and/or add reactions to messages. 
{% endhint %}



