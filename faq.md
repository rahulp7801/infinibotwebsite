---
description: Some frequently asked questions about InfiniBot.
---

# FAQ

## Is InfiniBot free?

Yes!!! All of InfiniBot's core features are available to the public for FREE! However, if you would like a more customized bot and extra features, be sure to donate to our Patreon! This will unlock more features for you and a server of your choice.

## How can I support InfiniBot?

It would be amazing if you could donate to our Patreon. You would be directly responsible for covering hosting costs and the bot's operational costs!



## How can I set up the bot for my server?

Run the following command:

```text
%setup all
```

This brings you to a painless, quick, 5-minute interactive setup session with InfiniBot! After this, you will not have to keep maintaining it, as the bot will do it on its own!

## Another bot has the same prefix, what can I do?

InfiniBot also automatically responds when you ping the bot as the prefix. If you have no other choice, you will have to modify one of the bots' prefix. To accomplish this with InfiniBot, run the following command:

```text
%changeprefix <prefix>

// example usage
%changeprefix !
```

{% hint style="info" %}
If you want the bot to have a word prefix, you **MUST** surround it in quotes during setup, due to a Discord limitation. 

**%changeprefix "yo "**

This would change the prefix to "yo ", so an example command would look like this:

**yo help**
{% endhint %}

## **How can I prevent members from using moderation commands?**

Luckily, InfiniBot has an in-built permission system, so only moderators can use moderation commands with the bot.

## How do I use interactions?

### Buttons

Interactions are a super cool new Discord feature that allows users to interact with bots in another way! 

#### For "Reaction" Roles

InfiniBot offers buttons for role-assignment instead of the traditional reaction roles. However, if you still prefer the latter, you can specify that during setup. This is set by using the command:

```text
%rr create
```

Buttons work similarly, and there isn't much to learn about them!



{% file src=".gitbook/assets/screenshot-2021-06-04-145717.png" caption="Using buttons for role assignment" %}

#### A Cool Calculator Feature

InfiniBot offers a calculator with a really nice GUI for users to interact with directly from the comfort of their server. Buttons make these possible!! 

#### Polls

InfiniBot incorporates buttons into polling, so it is easy to understand what you are voting for in a poll. 

### Slash Commands

Discord added a cool new way to interact with bots known as slash commands. To begin, start by typing a "/" into the chat bar, and a list of commands for bots that support this feature will show up!

#### Benefits

1. With slash commands, bots no longer have to be physically invited to a server \(coming soon, not yet though\) to be used.
2. Bots no longer have to read EVERY message to see if it contains a command, making it exponentially faster!!
3. Bots don't have to spam your DMs anymore, because slash commands support yet another new Discord feature known as ephemeral messages. To be brief, these messages can only be seen by the invoker, so it is similar to a DM in a sense.
4. You no longer have to struggle with learning all of the bot's commands, as each slash command comes with a description of what it is used for, and when to use it!
5. Gone are the days of remembering 5-6 prefixes for all of the bots in your server, they all now work with just one!

## Why does the bot ask for so many permissions?

InfiniBot has a moderation module that requires such permissions. Without them, the bot cannot perform actions such as **banning, muting, kicking, warning** and so on. 

## How do I know InfiniBot will not nuke my server?

InfiniBot is currently in alpha, and the goal is to become a large bot. If the bot nukes a server, those hopes would quickly be dashed as the devs and the bot itself would be banned from Discord :\(\(

