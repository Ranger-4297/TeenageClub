---
layout: default
title: Handbook
description: Command syntax & extra
permalink: handbook
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
    <summary class="text-primary">click to expand</summary>

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
Creates a log of the last 100  messages in the current channel. This includes deleted messages within an hour.
All logs can be found [here](https://yagpdb.xyz/manage/794236519543734273/logging/).
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command and view these links.
Normal uses of our server may also view these links. But will not be have adjacent perms such that they can see deleted messages.
#### Syntax

<pre style="background-color: #2a2a2a ;">
 <code>
  Logs [Count:Whole number]
 </code>
</pre>
<pre style="background-color: #2a2a2a ;">
 <code>
  [-channel channel:Channel - Optional channel to log instead]
 </code>
</pre>

---
## Undelete
#### Description
Views the last 10 recently deleted messages from the last hour.
By default it views *your* messages<br>
If you specify the <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-a </span> flag it views all users deleted messages<br>
Or, <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-u </span> to view a specific users deleted messages<br>
You need a staff role to use <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-a </span>&nbsp;& <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-u &nbsp;</span><br>
And <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-u &nbsp;</span> overrides <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-a &nbsp;</span><br>
You can also use a target channel with <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-channel &nbsp; </span>
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Undelete
 </code>
</pre>
<pre style="background-color: #2a2a2a ;">
 <code>
  [-a a:Switch - from all users]
  [-u u:Mention/ID - from a specific user]
  [-channel channel:Channel - Optional target channel]
 </code>
</pre>

---
## Clean
#### Description
Delete a specified number of messages from chat, optionally filtering by user, max age and regex or ignoring pinned messages.<br>
**Warning:** Using <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp; clean \<UserID> \<Amount> &nbsp;</span> does not work. This is because the user ID is interpreted as the amount. As it is over the limit of 100, it is treated as invalid.<br>
You can use <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp; clean \<Amount> \<UserID> &nbsp;</span> instead or mention the user.<br>
Specify a regex with <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp; -r regex_here &nbsp;</span> and max age with <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp; -ma maxage_here &nbsp;</span>
**Note:** Will only look in the last 1k messages
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Clean &lt;Num:Whole number&gt;
  Clean &lt;Num:Whole number&gt; &lt;User:Mention/ID&gt;
  Clean &lt;User:Mention/ID&gt; &lt;Num:Whole number&gt;
 </code>
</pre>
<pre style="background-color: #2a2a2a ;">
 <code>
  [-r r:Text - Regex]
  [-im im:Switch - Invert regex match]
  [-ma ma:Duration - Max age]
  [-minage minage:Duration - Min age]
  [-i i:Switch - Regex case insensitive]
  [-nopin nopin:Switch - Ignore pinned messages]
  [-a a:Switch - Only remove messages with attachments]
  [-to to:Whole number - Stop at this msg ID]
 </code>
</pre>

---
## Modinfo
#### Description
Allows staff members to view a users history on moderation. Includes username, userID, nickname,  account creation date & total number of each sanction.<br>
If provided the <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp; -n &nbsp;</span> flag, then does **not** show the sanction count.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Modinfo &lt;User:Mention/ID&gt;
 </code>
</pre>
<pre style="background-color: #2a2a2a ;">
 <code>
  [-n r:Switch - Doesn't show sanction count]
 </code>
</pre>

---
## Cases
#### Description
Shows all cases belonging to a user. Including warnings, mutes, kicks & bans.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Cases &lt;User:Mention/ID&gt; [page]
 </code>
</pre>

---
## Case
#### Description
Provides information on a moderative case, such as moderator, user, case type & reason.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Case &lt;Case:Case Number&gt;
 </code>
</pre>

---
## Delcase
#### Description
Deletes any given case.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Delcase &lt;Case:Case Number&gt;
 </code>
</pre>

---
## Warn
#### Description
Warns a user for a given reason. Stores the warning on our case system. 1st tier punishment on record.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Warn &lt;User:Mention/ID&gt; &lt;Reason:Text&gt;
 </code>
</pre>


---
## Mute
#### Description
Mute a user for a given reason & duration. Stores the mute on our case system. 2nd tier punishment on record.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Mute &lt;User:Mention/ID&gt; [Duration:Duration] [Reason:Text] 
  Mute &lt;User:Mention/ID&gt; [Reason:Text] [Duration:Duration] 
  Mute &lt;User:Mention/ID&gt; [Duration:Duration>]
  Mute &lt;User:Mention/ID&gt; [Reason:Text]
  Mute &lt;User:Mention/ID&gt;
 </code>
</pre>

---
## Unmute
#### Description
Unmutes a user for a given reason & duration. Stores the Unmute on our case system. 1st tier punishment removal.
#### Role(s) needed
Any & all moderators of our staff team have sufficient permissions to run the command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Unmute &lt;User:Mention/ID&gt; [Reason:Text]
 </code>
</pre>

---
## Kick
#### Description
Kicks a user for a given reason. Stores the Kick on our case system. 3rd tier punishment on record.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Trial Moderator'. 'Moderator's and above have permission to run this command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Kick &lt;User:Mention/ID&gt; [Reason:Text]
 </code>
</pre>
## Ban
#### Description
Bans a user for a given reason & duration. Stores the Ban on our case system. 4th tier punishment on record.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Trial Moderator'. 'Moderator's and above have permission to run this command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Ban &lt;User:Mention/ID&gt; [Reason:Text]
 </code>
</pre>
<pre style="background-color: #2a2a2a ;">
 <code>
  [-d d:Duration - Duration]
  [-ddays ddays:Whole number - Delete Days]
 </code>
</pre>

---
## Unban
#### Description
Unbans a user for a given reason. Stores the Unban on our case system. 2nd tier punishment removal.
#### Role(s) needed
This command is locked for those of our staff team ranking at 'Moderator' & below. 'Head Mod's and above have permission to run this command.
#### Syntax
<pre style="background-color: #2a2a2a ;">
 <code>
  Unban &lt;User:Mention/ID&gt; [Reason:Text]
 </code>
</pre>

---
## Extra/help
### Clean
#### Regex flag
The regex flag can be used to delete any messages containing a given word.<br>
For example: <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;Clean 100 -r "cum" &nbsp;</span>, <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;Clean 100 -r \bporn(.)hub\b &nbsp;</span><br>
The <span style="background-color: #2a2a2a; border-color: white; border-style: solid; border-width: 1px; border-radius: 4px">&nbsp;-i&nbsp; </span>just makes sure what you've given isn't case sensitive.<br>
I'd add this to most clean commands if you use the Regex flag

---

[Back to top](#welcome)