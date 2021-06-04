---
description: Configure InfiniBot to meet your server's specific needs!
---

# Configuration

## COMMANDS

{% hint style="info" %}
All of these commands can **ONLY** be run by a server moderator!
{% endhint %}

### Help

```text
%setup
```

This returns a help menu that shows all of the configuration commands.

### List

```text
%setup list
```

Shows a list of commands that can be used for configuration.

### Welcome Channel

```text
%setup welcomechannel <#channel>

// EXAMPLE USAGE:
%setup welcomechannel #welcome
```

This is a command that basically saves the channel that the bot will be sending welcome/goodbye messages to. The bot needs the **Read Messages, Send Messages, and Embed Links** permissions in said channel in order for it to work.

### Welcome Text / Welcome Message

```text
%setup welcometext <text>

// EXAMPLE USAGE:
%setup welcometext Hey {user}, welcome to {guild}!
```

InfiniBot offers a couple of parameters for your welcome message. They include the following:

| Variables | Output |
| :--- | :--- |
| {user} | The new user's username. |
| {member} | A **mention** of the joined user. |
| {guild} | The name of your server. |
| {members} | The count of members you have in your server. |

An example of throwing all of them together could include:  
**Hey {user}, welcome to {guild} where we have {members} members. Have a fun time {user}!**

Your welcome message will be sent as an embed in the welcome channel you specified.

### Welcome Nickname

```text
%setup welcomenick <nickname>

// EXAMPLE USAGE:
%setup welcomenick Peasant
```

The bot will change the new user's **nickname** to the specified nick. You must give the bot permission to **Manage Nicknames** for this feature to work.

### Minecraft Server IP

```text
%setup mcip <ip>

// EXAMPLE USAGE:
%setup mcip 127.0.0.1:5000
```

This was a highly requested feature, as many people play Minecraft and wanted to access/share the IP with a simple command.

### Leveling

```text
%setup levelups <True or False>

// EXAMPLE USAGE:
%setup levelups True
```

Toggles the leveling module accordingly. Aliases for this command include **XP,** and **levelups.**

### Ghost Ping Detection

```text
%setup ghostpingdetection <True or False>

// EXAMPLE USAGE:
%setup ghostpingdetection True
```

Another highly requested feature. InfiniBot can detect when a user ghost pings \(or attempts to ghost ping\) another user and publicly expose them in the chat.

### Private Welcome Message \(DM\)

```text
%setup privmsg <text>

// EXAMPLE USAGE:
%setup privmsg Have a fun time here in {guild}.
```

All of the variables for the welcome message work here as well. The bot will DM the user the message you specify here when they join. This is helpful for when your server is large and you won't have the time to explain to the user how everything works.

### Welcome Role

```text
%setup welcomerole <@role>

// EXAMPLE USAGE:
%setup welcomerole @Member
```

This is the role that the bot will assign to every member that joins the server. The bot requires the **Manage Roles** permission for this to work. If captcha is enabled, then the assignment of this role is delayed until the user successfully completes the captcha first.

### Blacklisted Words

```text
%setup blacklist <True or False>

// EXAMPLE USAGE:
%setup blacklist True
```

This enables/disables the plugin that can detect foul language. The bot deletes the message, sends a DM to the user explaining the reason, and adding an infraction to the user's tab. The bot requires the **Manage Messages** permission for this plugin to work.

### Goodbye Message

```text
%setup leavemsg <text>

// EXAMPLE USAGE:
%setup leavemsg Goodbye {user}, hopefully you come back soon.
```

This message will be sent in the same message as the welcome messages are sent. All of the variables remain the same as the welcome message.

### Starboard Channel

```text
%setup starboardchannel <#channel>

// EXAMPLE USAGE:
%setup starboardchannel #general
```

Every good server needs a starboard. So, InfiniBot has a starboard plugin that can automatically detect when a message has a certain amount of stars \(determined by a moderator\) and send the message as an embed in the starchannel. It is like pinning a message, but members have the power too!

### Server Captcha

```text
%setup servercaptcha <True or False>

// EXAMPLE USAGE:
%setup servercaptcha True
```

If you set up a welcome role, the assignment of that role to the member will be delayed until they can successfully complete a captcha that is DMed to them when they join. If they can get it correct within three guesses, they get the role. Otherwise, they will remain unverified until a server moderator manually assigns them the role.

### Spam Detection

```text
%setup spamdetect <True or False>

// EXAMPLE USAGE:
%setup spamdetect False
```

InfiniBot can automatically detect when a user is spamming. If you set up a muterole, then the bot will automatically mute the person who is spamming.

### Logging

```text
%setup logging <True or False>

// EXAMPLE USAGE:
%setup logging True
```

This command toggles logging, and after you choose whether you want it on or off, depending on your choice, you will be prompted to select the channel in which you want these logs to be sent to. The bot logs information such as joins/leaves, mutes/warns/kicks/bans, and so on.

### Mute Role

```text
%setup muterole <name>

// EXAMPLE USAGE:
%setup muterole Muted
```

This command tells the bot to create a mute role and update permissions for the role so a person who has it cannot talk in the chat. The bot requires the **Manage Roles** and the **Manage Channels** permissions for this command.

### Prefix

```text
%changeprefix <prefix>

// EXAMPLE USAGE:
%changeprefix !
```

InfiniBot features a customizable prefix, so you can make sure that it does not interfere with other bots.

{% hint style="info" %}
If you wish to have a word as your prefix, you must surround it in quotes and a space due to a Discord limitation.

%changeprefix "yo "
{% endhint %}

### ALL OF THE ABOVE

```text
%setup all
```

This command takes you through all of the above commands in 5 or so minutes, it is an interactive experience that is meant to be easy on the user. **THIS IS THE RECOMMENDED WAY TO SET UP THE BOT!** 

