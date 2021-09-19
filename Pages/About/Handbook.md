---
layout: default
title: Handbook
description: Command syntax & extra
permalink: Commandbook
---

![TCModeration-Guides](https://ranger-4297.github.io/TeenageClub/assets/images/titles/TCCH.png)


Largely copied/pasted help commands
I couldn't really be arsed to make my own descriptions.

---

# Welcome!
This document/handbook contains a full, complete and updated list of all moderation commands & how to use them in TeenageClub.
This includes commands like undelete and clean.

---

## Contents

<details>
    <summary class="text">click to expand</summary>

<ul>
  <li><a href="#logs">Logs</a>
    <ul>
    <li><a href="#description">Description</a></li>
    <li><a href="#roles-needed">Role(s) needed</a></li>
    <li><a href="#syntax">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#undelete">Undelete</a>
    <ul>
    <li><a href="#description-1">Description</a></li>
    <li><a href="#roles-needed-1">Role(s) needed</a></li>
    <li><a href="#syntax-1">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#clean">Clean</a>
    <ul>
    <li><a href="#description-2">Description</a></li>
    <li><a href="#roles-needed-2">Role(s) needed</a></li>
    <li><a href="#syntax-2">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#modinfo">Modinfo</a>
    <ul>
    <li><a href="#description-3">Description</a></li>
    <li><a href="#roles-needed-3">Role(s) needed</a></li>
    <li><a href="#syntax-3">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#cases">Cases</a>
      <ul>
    <li><a href="#description-4">Description</a></li>
    <li><a href="#roles-needed-4">Role(s) needed</a></li>
    <li><a href="#syntax-4">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#case">Case</a>
    <ul>
    <li><a href="#description-5">Description</a></li>
    <li><a href="#roles-needed-5">Role(s) needed</a></li>
    <li><a href="#syntax-5">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#delcase">DelCase</a>
    <ul>
    <li><a href="#description-6">Description</a></li>
    <li><a href="#roles-needed-6">Role(s) needed</a></li>
    <li><a href="#syntax-6">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#warn">Warn</a>
    <ul>
    <li><a href="#description-7">Description</a></li>
    <li><a href="#roles-needed-7">Role(s) needed</a></li>
    <li><a href="#syntax-7">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#mute">Mute</a>
    <ul>
    <li><a href="#description-8">Description</a></li>
    <li><a href="#roles-needed-8">Role(s) needed</a></li>
    <li><a href="#syntax-8">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#unmute">Unmute</a>
    <ul>
    <li><a href="#description-9">Description</a></li>
    <li><a href="#roles-needed-9">Role(s) needed</a></li>
    <li><a href="#syntax-9">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#kick">Kick</a>
    <ul>
    <li><a href="#description-10">Description</a></li>
    <li><a href="#roles-needed-10">Role(s) needed</a></li>
    <li><a href="#syntax-10">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#ban">Ban</a>
    <ul>
    <li><a href="#description-11">Description</a></li>
    <li><a href="#roles-needed-11">Role(s) needed</a></li>
    <li><a href="#syntax-11">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#unban">Unban</a>
    <ul>
    <li><a href="#description-12">Description</a></li>
    <li><a href="#roles-needed-12">Role(s) needed</a></li>
    <li><a href="#syntax-12">Syntax</a></li>
    </ul>
  </li>
  <li><a href="#extrahelp">Ex</a>
    <ul>
    <li><a href="#clean">Clean</a></li>
      <ul>
        <li><a href="#regex-flag">Regex flag</a></li>
      </ul>
    </ul>
  </li>
</ul>
</details>


---
## Logs
#### Description
Creates a log of the last messages in the current channel. This includes deleted messages within an hour.
All logs can be found [here](https://yagpdb.xyz/manage/794236519543734273/logging/).
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command and view these links.
Normal uses of our server may also view these links. But will not be have adjacent perms such that they can see deleted messages.
#### Syntax
```
Logs [Count:Whole number]
```
```
[-channel channel:Channel - Optional channel to log instead]
```
---
## Undelete
#### Description
Views the first 10 recent deleted messages. By default, only the current user's deleted messages will show. You can use the `-a` flag to view all users delete messages, or `-u` to view a specified user's deleted messages. Both `-a` and `-u` require Manage Messages permission. **Note:** `-u` overrides -a meaning even though `-a` might've been specified along with `-u` only messages from the user provided using `-u` will be shown.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Undelete 
```
```
[-a a:Switch - from all users]
[-u u:Mention/ID - from a specific user]
[-channel channel:Channel - Optional target channel]
```
---
## Clean
#### Description
Delete the last number of messages from chat, optionally filtering by user, max age and regex or ignoring pinned messages. 
**Warning:** Using `clean <userId> <amount>` does not work. This is because the user ID is interpreted as the amount.
As it is over the limit of 100, it is treated as invalid. You can use `clean <amount> <userId>` instead or mention the user.
Specify a regex with `-r regex_here` and max age with `-ma 1h10m`
You can invert the regex match (i.e. only clear messages that do not match the given regex) by supplying the `-im` flag **Note:** Will only look in the last 1k messages
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Clean <Num:Whole number>
Clean <Num:Whole number> <User:Mention/ID>
Clean <User:Mention/ID> <Num:Whole number>
```
```
[-r r:Text - Regex]
[-im im:Switch - Invert regex match]
[-ma ma:Duration - Max age]
[-minage minage:Duration - Min age]
[-i i:Switch - Regex case insensitive]
[-nopin nopin:Switch - Ignore pinned messages]
[-a a:Switch - Only remove messages with attachments]
[-to to:Whole number - Stop at this msg ID]
```
---
## Modinfo
#### Description
Allows staff members to view a users information for moderation. Includes username, userID, nickname,  account creation date & total number of each sanction.
If provided the `-n` flag, then does not show the sanction count.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Modinfo <User:Mention/ID>
```
```
[-n r:Switch - Doesn't show sanction count]
```
---
## Cases
#### Description
Shows all cases belonging to a user. Includes warnings, mutes, unmutes, kicks & bans.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Cases <User:Mention/ID> [page]
```
---
## Case
#### Description
Provides information on a moderative case, such as moderator, user, case type & reason.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Case <Case:Case Number>
```
---
## Delcase
#### Description
Deletes any given case.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Delcase <Case:Case Number>
```
## Warn
#### Description
Warns a user for a given reason. Stores the warning on our case system. 1st tier punishment on record.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Warn <User:Mention/ID> <Reason:Text>
```
---
## Mute
#### Description
Mute a user for a given reason & duration. Stores the mute on our case system. 2nd tier punishment on record.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Mute <User:Mention/ID> [Duration:Duration] [Reason:Text] 
Mute <User:Mention/ID> [Reason:Text] [Duration:Duration] 
Mute <User:Mention/ID> [Duration:Duration>]
Mute <User:Mention/ID> [Reason:Text]
Mute <User:Mention/ID>
```
---
## Unmute
#### Description
Unmutes a user for a given reason & duration. Stores the Unmute on our case system. 1st tier punishment removal.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
```
Unmute <User:Mention/ID> [Reason:Text]
```
---
## Kick
#### Description
Kicks a user for a given reason. Stores the Kick on our case system. 3rd tier punishment on record.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Trial Moderator'. 'Moderator's and above have permission to run this command.
#### Syntax
```
Kick <User:Mention/ID> [Reason:Text]
```
## Ban
#### Description
Bans a user for a given reason & duration. Stores the Ban on our case system. 4th tier punishment on record.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Trial Moderator'. 'Moderator's and above have permission to run this command.
#### Syntax
```
Ban <User:Mention/ID> [Reason:Text]
```
```
[-d d:Duration - Duration]
[-ddays ddays:Whole number - Delete Days]
```
---
## Unban
#### Description
Unbans a user for a given reason. Stores the Unban on our case system. 2nd tier punishment removal.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Moderator' & below. 'Head Mod's and above have permission to run this command.
#### Syntax
```
Unban <User:Mention/ID> [Reason:Text]
```
---
## Extra/help
### Clean
#### Regex flag
The regex flag can be used to delete any messages containing a given word. For example: `Clean 100 -r "cum"` OR anything that isn't AlphaNumerical (Alphabet & Numbers) you could do `Clean 100 -r "/[^a-zA-Z\d\s:\u00C0-\u00FF]/g`"
        Regex case insensitive
The just makes sure what you've given isn't case sensitive. I'd add this to most clean commands if you use the Regex flag

---

[Back to top](#welcome)