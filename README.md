# Project: Lotus

![Project:Lotus-Title]()

## Disclaimer

Project: Lotus is not affiliated with Among Us or Innersloth LLC, and the content contained therein is not endorsed or otherwise sponsored by Innersloth LLC. Portions of the materials contained herein are property of Innersloth LLC. © Innersloth LLC. 

![Discord]()

<p align="center"><a href=""><img src=""></a></p>

## Releases

AmongUs Version: **2023.2.28**
**Latest Version: [Here]()**

## Regarding This Mod

Project: Lotus (The Mod) is considered a Host Only Mod (or, Host Only Environment). This means that only The Host needs to install the mod (on a Windows Operating System) for it to work. Once The Host creates a modded lobby, clients (players) from any device are able to join and enjoy The Mod.<br>

#### The Following Restriction(s) Apply<br>

- If The Host leaves in the middle of a game, The Mod will no longer work (i.e. the roles will no longer function as intended). This happens regardless of whether the client is modded (has joined with The Mod) or not (termed 'vanilla').<br>

#### Benefits Of Being A Modded Client.<br>

- Custom start screen displaying Role Name & Ability/Win Condition (Victory Parameters)
- Detailed results display featuring player avatars & their game stats
- Custom victory screen reflecting the Role's unique win condition.
- Ability to view additional settings in lobby. 
- Custom buttons in game.
- More detailed task log.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Features

## Hotkeys (Host Only)

#### Usable in Game
| Function                       | HotKey               |
| ------------------------------ | -------------------- |
| Terminate the game             | `Shift`+`L`+`Enter`  |
| Skip meeting to end            | `Shift`+`M`+`Enter`  |
| Force meeting                  | `RShift`+`M`+`Enter` |


#### Usable In Meeting 
| Function                               | HotKey           |
| -------------------------------------- | ---------------- |
| Execute clicked player                 | `Ctrl`+`RMB`     |
| Sends *certain* messages to all        | `LShift`+`Enter` |
| Sends *certain* messages to dead       | `RShift`+`Enter` |


#### Usable During Countdown
| Function                       | HotKey      |
| ------------------------------ | ----------- |
| Cancel game start & autoplay   | `C`         |
| Start the game immediately     | `Shift`     |


#### Usable In Settings
| Function                       | HotKey              |
| ------------------------------ | ------------------- |
| Reset default settings/options | `Ctrl`+`Delete`     |


#### Usable In Lobby
| Function                       | HotKey         |
| ------------------------------ | -------------- |
| Reload Lang file updates       | `Ctrl` + `T`   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Hotkeys (Mod Clients Only)

#### Usable In Lobby
| Function                       | HotKey          |
| ------------------------------ | --------------- |
| Next page in option shower     | `Tab`           |
| Previous page in option shower | `LCtrl` + `Tab` |

#### Usable In Chat
| Function                               | HotKey             |
| -------------------------------------- | ------------------ |
| Paste the text                         | `Ctrl`+`V`         |
| Go back in time of chat send history   | `↑`                |
| Go future in time of chat send history | `↓`                |

#### Usable Anywhere
| Function                         | HotKey       |
| -------------------------------- | ------------ |
| Increase Resolution              | `Ctrl`+`+`   | 
| Decrease Resolution              | `Ctrl`+`-`   |
| Output log to desktop            | `Ctrl`+`F1`  |              

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Chat Commands

#### Host Only

| Function                         | Command                    | Aliases     |
| -------------------------------- | -------------------------- | ----------- |
| Shows all players and their IDs  | `/id`                      |             |
| Displays message to ALL players  | `/say [msg]`               | `/s`        |
| Kicks the provided player        | `/kick [name \| id]`       |             |
| Bans the provided player         | `/ban [name \| id]`        |             |
| Creates a log dump               | `/dump`                    |             |


### All Clients

#### About The Most Recent Game
| Function                           | Command       | Aliases            |
|------------------------------------|---------------|--------------------|
| Show Game Results                  | `/lastresult` | `/l`               |
| Show Winner                        | `/winner` or  | `/win`             |

#### Configurable Commands
| Function                           | Command                            |
|------------------------------------|------------------------------------|
| Change My Color                    | `/color`                           |
| Change My Level                    | `/level`                           |
| Change My Name                     | `/name`                            |

#### General Lobby/Game Info
| Function                           | Command              | Aliases     |
|------------------------------------|----------------------|-------------|
| Show Active Roles Settings         | `/now roles`         | `/n r`      |
| Show Active Settings               | `/now`               | `/n`        |
| Show Attribute Description         | `/help attributes`   | `/helpatt`  |
| Show Mode Description              | `/help modes`        | `/helpm`    |
| Show % for All Roles > 0%          | `/perc`              |             |
| Show Role Description              | `/roles [Role]`      | `/r [Role]` |


#### Player Info In Game
| Function                           | Command         | Aliases     |
|------------------------------------|-----------------|-------------|
| Show Basic Role Description        | `/myrole`       | `/m`        |
| Show Current Role Option           | `/options`      | `/o`        |
| Show Full Role Description         | `/descriptions` | `/desc`     |


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Templates

__Location__: `LOTUS_DATA/Templates.yaml`<br>
__Chat Command__: /t _or_ /template _or_ /templates [TAG]<br>

Templates allow you to send pre-written and frequently used blocks of text in chat. They offer endless possibilities and are commonly used for various purposes, such as welcome messages, rules, first meeting messages, and commonly used statements.

To access your saved templates, you or another player can type /t [tag] (e.g. /t rules). If the host types the message, the tag will be hidden (so no one will know you are using it to show messages), but the text will be shown to everyone. If a player types the same command, the tag will show for everyone, but the message will be shown privately (only to the player).


#### Command Guide

This table serves as a quick reference for the different tags and their corresponding descriptions. The host can use tags to customize the lobby and help players understand the game.

| Command                      | Alias                 | Description                                                    |
| ---------------------------- | --------------------- | -------------------------------------------------------------- |
| `/t list`                    | `/t l`                | Lists all templates by ID (and their tags)                     |
| `/t tags`                    |                       | Shows all tags built into the mod                              |
| `/t variables`               | `/t v`                | Shows all variables that can be used in templates              |
| `/t reload`                  |                       | Reloads all templates                                          |
| `/t [tag]`                   | `/[alias]`            | Shows template to all players                                  |
| `RShift`+`/t [tag]`          | `RShift`+`/[alias]`   | Shows template to dead players                                 |

#### Tag Customization 

Project Lotus has a number of built-in tags. These tags will automatically be displayed when certain lobby/meeting events happen. These are optional, but allow you to further customize your lobby.

| Tag                |  Description                                                                                                                                                                                |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| modifier-info      | The template is used by the @ModsDescriptive tag when displaying modifiers. This template uses ^Role_XXX variables to display its  information.                                             |
| lobby-join         | Tag for the template shown to players joining the lobby.                                                                                                                                    |
| autostart          | Template triggered when the autostart timer begins.                                                                                                                                         |
| meeting-first      | The template to show during the first meeting.                                                                                                                                              |
| meeting-subsequent | The template to show during all meetings after the first.                                                                                                                                   |
| meeting-start      | The template to show during each meeting.                                                                                                                                                   |

### Usable Variables

This table serves as a quick reference for the different variables that can be utilized in templates.

| Name             | Variable           | Output                                                                                              |
| ---------------- | ------------------ | --------------------------------------------------------------------------------------------------- |
| Room Code        | ${RoomCode}        | The current room code                                                                               |
| Host             | ${Host}            | The host's name                                                                                     |
| AU Version       | ${AUVersion}       | The current version of Among Us                                                                     |
| Mod Version      | ${ModVersion}      | The current mod version                                                                             |
| Mod Name         | ${ModName}         | The current mod name                                                                                |
| Map              | ${Map}             | The name of the last map selected                                                                   |
| Game Mode        | ${Gamemode}        | The current game mode selected                                                                      |
| Date             | ${Date}            | The current date (based on host)                                                                    |
| Time             | ${Time}            | The current time (based on host)                                                                    |
| Players          | ${Players}         | A list of player names separated by a comma                                                         |
| Player Count     | ${PlayerCount}     | A count of all players currently in lobby                                                           |
| All Roles        | ${AllRoles}        | A categorized list of all roles in the mod                                                          |  
| All Modifiers    | ${AllModifiers}    | A list of all modifiers in the mod                                                                  |
| My Role          | ${MyRole}          | Echoes the text of /myrole which shows the player's role and role description.                      |
| Name             | ${Name}            | The player's name                                                                                   |
| Color            | ${Color}           | The color of the player's avatar                                                                    |
| Role             | ${Role}            | The player's role                                                                                   |
| Blurb            | ${Blurb}           | The player's role blurb                                                                             |
| Description      | ${Description}     | The player's role description                                                                       |
| Options          | ${Options}         | The player's role options                                                                           |
| Faction          | ${Faction}         | The player's faction                                                                                |
| Modifiers        | ${Modifiers}       | Shows the player's modifiers as a list of names                                                     |
| Mods Descriptive | ${ModsDescriptive} | Displays descriptive info about each of a player's modifiers                                        |


### Template Customization

There are endless possibilities when it comes to template customization in Project: Lotus. Not only are all the variables above usable in any templates created by the host, hosts can also use HTML and symbols to customize their templates even further. 

Here are some basic tools to get you started:

#### Usable HTML Tags 

| HTML Tag       | Description                                            |
| -------------- | ------------------------------------------------------ |
| `<b>`          | Bold text                                              |
| `<i>`          | Italicized text                                        |
| `<u>`          | Underlined text                                        |
| `<s>`          | Strikethrough text                                     |
| `<sub>`        | Subscript text                                         |
| `<sup>`        | Superscript text                                       |
| `<mark>`       | Highlighted or marked text                             |
| `<size= >'     | Size of text (Default AU size is 2)                    |
| `<color= >`    | Color of the text (use hex code)                       |


#### Usable Unicode Symbols

★ ☀ ☂ ☆ ☹ ☺ ♥ ♡ ♩ ♪ ♫ ♬ ✓ ♠ ◈ ☎ ♀ ♂ ☜ ☝ ☞ ☟ ☯ ☃ ✿ ❀ ☁ ¿ ※ ⁑ ∞ ≠ + ÷ º 乂 ⁂ ¤ § ∮ 彡 个 《 「 」 人 요 〖 〗 ロ 米 卄 王 ī l 【 】 · ㅇ ° ◆ ◇ ◥ ◤ ◢ ◣ 《 》 ︵︶

#### Blank Template

```
Templates:
- Tag:
  Aliases: []
  Title:
  Text:
```

#### Default Template 

```
Templates: #This is necessary for the file, do not remove this line!


- Tag: lobby-join #Notice that there is a hyphen (-) before the Tag, it is necessary when creating new tags. This is the text entered after '/t'
  Aliases: [welcome] #Aliases can be used to create custom commands (i.e. no need for '/t'). This Alias allows for '/welcome' to generate the same response as '/t lobby-join'
  Title: <color=#e9b915>Welcome ${Name}</color> #This is the text that will appear in place of the host's name at the top of the message in chat. 
  Text: | #This pipe (|) allows for conditional formatting (line breaks can easily be attained by pressing enter). Each line MUST have one space indented from the 'Text:' column
   ===================
   This is a modded lobby hosted by ${Host}. 

   <b>Mod Version:</b> Project: Lotus v${ModVersion}

   Use '/help' for a list of available chat commands.

   Enjoy!



- Tag: rules
  Aliases: [rules]
  Title: Lobby Rules
  Text: #Fill this in with your lobby rules. Some examples for this could be 'do not claim roles unless you have important info' or 'saying start results in auto-kick' 



- Tag: meeting-first
  Title: Your Role Information
  Text: |
    ===================
    ${Role} (${Faction}):
    ${Blurb}
    ${Description}

    ${ModsDescriptive}



- Tag: meeting-start
  Title: Helpful Commands
  Text: |
   =================
    /m → show your role & modifier description
    /o → view your role and modifier options
    /r [role] → other roles' description & options
    /desc → first meeting message
    /help → list of helpful commands
```

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Default lobby-join Template
![lobby-join](https://cdn.discordapp.com/attachments/1117632307487064145/1117942315974135868/image.png)

#### Default meeting-first Template
![meeting-first](https://cdn.discordapp.com/attachments/1117632307487064145/1117919318538211429/image.png)

#### Default meeting-start Template
![meeting-start](https://cdn.discordapp.com/attachments/1117632307487064145/1117913469526749255/Standard_Meeting-Start_.png)

#### Useful Templates Not Included With Defaults

##### Nicer meeting-first Template
```
- Tag: meeting-first
  Title: "${Role} (${Faction})\n<sup>Modifiers: ${Modifiers}"
  Text: |
   \n================
  
   You are the ${Role}

   ${Description}

   ${ModsDescriptive}
```

##### Helpful Alchemist Templates
```
- Tag: ai
  Aliases: [ai]
  Title: Alchemist Ingredient List
  Text: |
   ------------------------------------------------------
    <color=#89a0a0>◆ = Catalyst</color> (Source: Completing Tasks)
    <color=#d15914>Θ = Theta Rift</color> (Source: Random Spawn)
    <color=#96c185>⚠ = Vial of Decay</color> (Source: Dead Bodies)
    <color=#ffaced>❀ = Shifting Rose</color> (Source: Shapeshifters)
    <color=#8c28bc>☀ = Essence of Sight</color> (Source: Fixing Lights)
    <color=#72ff75>◯ = Fragment of Discussions</color> (Source: Groups of 3 or more people)
- Tag: ap
  Aliases: [ap]
  Title: Alchemist Potions:
  Text: |
   ------------------------------------------------------
    <color=#96c15b>Potion of Death</color>:
    Kills the nearest player

    <color=#d4d45e>Castling Brew</color>:
    Applies a 1-time use shield to the player

    <color=#9900ff>Potion of Sight</color>:
    Increases players vision for 60 seconds OR removes sabotage vision

    <color=#ff389b>Warp Potion</color>
    Teleports you and a random player

    <color=#0000ff>Mechanic's Mix</color>:
    Allows player to instant fix next sabotage

    <color=#6a8759>Leader Potion</color>:
    Gives +1 vote during the next meeting

    <color=#FFEDF9>S</color><color=#FFE4F4>e</color><color=#FFDCEE>r</color><color=#FFD4E8>e</color><color=#FFCBE2>n</color><color=#FFC3DC>e</color><color=#FFBBD7> </color><color=#FFB2D1>G</color><color=#FFAACB>r</color><color=#FFA2C5>a</color><color=#FF99BF>c</color><color=#FF91BA>e</color>: 
    Reveals the role of the most nearby player

    <color=#FF0000>U</color><color=#FF2A00>n</color><color=#FF5500>s</color><color=#FF7F00>t</color><color=#FFA301>a</color><color=#FFC702>b</color><color=#FFEB04>l</color><color=#AAF102>e</color><color=#55F801> </color><color=#00FF00>C</color><color=#00D455>o</color><color=#00AAA9>n</color><color=#007FFF>c</color><color=#0055FF>o</color><color=#002AFF>c</color><color=#0000FF>t</color><color=#2A00FF>i</color><color=#5400FF>o</color><color=#7F00FF>n</color>:
    Mutates into a random potion"
- Tag: api
  Aliases: [api]
  Title: Alchemist Potion Ingredients
  Text: |
   ------------------------------------------------------
    <color=#96c15b>Potion of Death</color>: <color=#96c185>
    ⚠ Vial of Decay</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
    
    <color=#d4d45e>Castling Brew</color>:
    <color=#89a0a0>(2) ◆ Catalyst</color> +  <color=#89a0a0>◆ Base Catalyst Amount</color>
    
    </color=#9900ff>Potion of Sight</color>:
    <color=#8c28bc>☀ = Essence of Sight</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
     
    <color=#ff389b>Warp Potion</color>:
    <color=#d15914>Θ = Theta Rift</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
     
    <color=#0000ff>Mechanic's Mix</color>:
    <color=#72ff75>◯ = Fragment of Discussions</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
    
    <color=#6a8759>Leader Potion</color>:
    <color=#72ff75>◯ = Fragment of Discussions</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
    
    <color=#FFEDF9>S</color><color=#FFE4F4>e</color><color=#FFDCEE>r</color><color=#FFD4E8>e</color><color=#FFCBE2>n</color><color=#FFC3DC>e</color><color=#FFBBD7> </color><color=#FFB2D1>G</color><color=#FFAACB>r</color><color=#FFA2C5>a</color><color=#FF99BF>c</color><color=#FF91BA>e</color>:
    <color=#ffaced>(2) ❀ Shifting Rose</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
    
    <color=#FF0000>U</color><color=#FF2A00>n</color><color=#FF5500>s</color><color=#FF7F00>t</color><color=#FFA301>a</color><color=#FFC702>b</color><color=#FFEB04>l</color><color=#AAF102>e</color><color=#55F801> </color><color=#00FF00>C</color><color=#00D455>o</color><color=#00AAA9>n</color><color=#007FFF>c</color><color=#0055FF>o</color><color=#002AFF>c</color><color=#0000FF>t</color><color=#2A00FF>i</color><color=#5400FF>o</color><color=#7F00FF>n</color>:
    <color=#d15914>(2) Θ Theta Rift</color> + <color=#89a0a0>◆ Base Catalyst Amount</color>
```

### Note On Template Creation
- The hyphen (-) is required
- The colon and space after it are required 
- The indentation of the word Text (aligning with the indentation of the word Tag) is required 
- You must capitalize Tag and Text (and any other parameter used in Template.yaml)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Friends

The native Among Us friends list is often considered pointless. However, with this system, you can create your own custom friend list easily using simple commands through the command line.

The friend list information is stored in the file `LOTUS_DATA/Friends.txt`.

### Added Friends List (Static File)

Commands:

| Command                     | Function                                        |
| --------------------------- | ----------------------------------------------- |
| `/friend add [playerId]`    | Adds a friend based on their player ID (1 - 15) |
| `/friend add [name]`        | Adds a friend based on their username           |
| `/friend remove [index]`    | Removes a friend based on their list position   |
| `/friend list`              | Lists all friends                               |


## Other Useful Commands

Here are some additional commands that you might find useful:

- `/kick [id]`: Kick a player based on their ID.
- `/ban [id]`: Ban a player based on their ID.

Use `/kick` or `/ban` without specifying an ID to obtain a list of available player IDs.

## Custom Tags

__Location__: `LOTUS_DATA/Titles'<br>
__File Type__: yaml<br>
__File Name__: Among Us Friend Code (e.g. envykindly#7034)<br>

Custom tags allow for players to add colors to their username as well as titles above their username in Among Us. In order for a host to add a players custom tag, they'll need to create a yaml file with any/all of the following information: 

```
UpperText:
 Text: # This is the text that goes above your username
 Gradient: # Creates a gradient FROM Color 1 to Color 2 automatically
 Size: # Default AU size is 2
  
Name: # This is the size and color/gradient attributed to your username. Leave this line blank and fill in the options below 
 Gradient: # Creates a gradient from Color 1 to Color 2 automatically. For gradient enter "[hex 1], [hex 2]" (refer to examples above)
 Size: # Default AU size is 2

Prefix: # This is the size, color, and text that goes before your username. Leave this line blank and fill in the options below
 Spaced: # This field is either True or False and used if there should be a space between the Suffix and the player's username (example: ♥ shiftyrose)
 Text: # Add the text you'd like to go before your username here   
 Color: # Add the hex code that you'd like the prefix to be here
 Size: # Default AU size is 2

Suffix: # This is the size, color, and text that goes after your username. Leave this line blank and fill in the options below
 Spaced: # This field is either True or False and used if there should be a space between the Suffix and the player's username (example: shiftyrose ♥)
 Text: # Add the text you'd like to go before your username here   
 Color: # Add the hex code that you'd like the prefix to be here
Size: # Default AU size is 2

LowerText:
 Text: # This is the text that goes below your username
 Gradient: # Creates a gradient FROM Color 1 to Color 2 automatically
 Size: # Default AU size is 2
```

__Creating A New Title__:<br>
Navigate to the `/LOTUS_DATA/Titles` directory<br>
Create a new yaml file named: `[friendcode].yaml` (example: `buffdulcet#0871.yaml`)<br>
Setup the title components in the yaml<br>

__Available Components__:<br>
UpperText - Responsible for the text above the player's username<br>
LowerText - Responsible for the text below the player's username<br>
Prefix - The text that comes before a player's username<br>
Suffix - The text that comes after a player's username<br>
Name - The player's username

__Component Items__: (These are the things you can define for each component to change)<br>
Text - Sets the text for the component (does not work for Name)<br>
Gradient - A list of HTML color codes defining a range of colors to apply to the text. (refer to example image)<br>
Color - If gradient is not specified, a solid color to apply to the text<br>
Size - The size of the text (default is 2)<br>
Spaced - (Only applicable to Prefix & Suffix) whether the text should have a space between it and the player's name<br>

Lastly you can reload your (local) title files with the command /t reload, the change is __immediate__<br>

### Example Tags

#### Example 1

UpperText:<br>
> Text: The One Above All<br>
> Gradient: "#ff0000, #e1e100" #Creates a gradient FROM Color 1 to Color 2 automatically<br>
> Size: 2 # Default AU size is 2, i believe this is exponential (so 100 would be terrible)<br>
  
Name:<br>
> Gradient: "#e1e100, #ff0000" #Creates a gradient FROM Color 1 to Color 2 automatically<br>
> Size: 2 # Default AU size is 2, i believe this is exponential (so 100 would be terrible)<br>

Prefix:<br>
> Spaced: True # If there should be a space between the Suffix and the player's name (example: Akali ♥)<br>
> Text: ∞    <br>
> Color: "#ff0000"<br>
> Size: 2 # Default AU size is 2, i believe this is exponential (so 100 would be terrible)<br>

Suffix:<br>
> Spaced: True # If there should be a space between the Suffix and the player's name (example: Akali ♥)<br>
> Text: ∞    <br>
> Color: "#e1e100"<br>
> Size: 2 # Default AU size is 2, i believe this is exponential (so 100 would be terrible)<br>
  
__Output__:<br>
![Alt text](https://cdn.discordapp.com/attachments/1034687568643641354/1117295347434266674/image.png)

#### Example 2

Name:<br>
> Gradient: "#3BCFD4, #FC9305, #F20094"

UpperText:<br>
> Size: 1.925<br>
> Text: ♡ Tipsy ♡<br>
> Gradient: "#3BCFD4,#F20094, #F74B4B, #FC9305,#96B373, #3BCFD4,#F20094"<br>

Prefix:<br>
> Text: ♥<bR>
> Spaced: true<br>
> Color: "#F20094"<br>

Suffix:<br>
> Text: ♥<br>
> Spaced: true<br>
> Color: "#3BCFD4"<br>

__Output__:<br>
![Alt text](https://media.discordapp.net/attachments/1109172438006235278/1116595347293220894/Screenshot_2023-05-31_181524.png)

# General Settings

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Admin Options

|               Name                     |                                              Description                                                     |     Type     |  Default  |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------ | :----------: | :-------: |
| Host GM                                | Allows Host to spawn as a GM. This makes them a ghost from the start of the game without any roles or tasks. |    Toggle    |    OFF    |
| Chat AutoKick                          | Automatically kick players who say certain banned words from game.                                           |    Toggle    |  DISABLED |
| Kick Players w/o Friendcodes           | Automatically kick players who do not have a friendcode from game.*                                          |    Toggle    |  DISABLED |
| Kick Players Under Level               | Automatically kick players who are below the defined level.                                                  |    Number    |  DISABLED |
| Kick Mobile Players                    | Automatically kick players who are playing on a mobile device.                                               |    Toggle    |  DISABLED | 
| AutoStart                              | Automatically starts the game when the set number of players is reached.                                     |    Number    |  DISABLED |
 
*This setting must be disabled if playing on a modded server.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Gameplay Options

|               Name                     |                                              Description                                                         |     Type     |  Default  |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | :----------: | :-------: |
| Optimize Role Counts for Playability   |                                                                                                                  |    Toggle    |    ON     |
| Fix First Kill Cooldown                | Overrides roles' first kill cooldown to match the one defined for their role instead of the automatic 10 seconds |    Toggle    |    ON     |
| Disable Tasks                          | Allows the host to disable certain tasks from showing up for players.                                            |    Toggle    |    OFF    |
| ┣ Disable Card Swipe                   | Disables the Card Swipe task from being given to players.                                                        |    Toggle    |    OFF    |
| ┣ Disable Med Scan                     | Disables the Med Scan task from being given to players.                                                          |    Toggle    |    OFF    |
| ┣ Disable Unlock Safe                  | Disables the Unlock Safe task from being given to players. (Task is only available on Airship)                   |    Toggle    |    OFF    |
| ┣ Disable Upload Data                  | Disables the Download/Upload Data task from being given to players.                                              |    Toggle    |    OFF    |
| ┣ Disables Start Reactor               | Disables the Start Reactor task from being given to players.                                                     |    Toggle    |    OFF    |
| ┗ Disable Reset Breaker                | Disables the Reset Breaker task from being given to players. (Task is only available on Airship)                 |    Toggle    |    OFF    |
| Disable Task Win                       | Disables the ability for Crewmates to win by completing all of their tasks.                                      |    Toggle    |    OFF    |
| Ghosts See Roles                       | Allows Ghosts (dead players) to see everyone's roles.                                                            |    Toggle    |    ON     |
| Ghosts See Indicators                  | Allows Ghosts to see indicators (symbols or text) next to players' names.*                                       |    Toggle    |    ON     |
| Ghosts Ignore Tasks                    | Allows for Crewmates to get a task win even if Ghosts do not finish their tasks.                                 |    Toggle    |    OFF    |
| Sync Meetings                          | Forces a global maximum number of meetings that can be called instead of each player having their own maximum.   |    Number    |   NEVER   | 

*Indicators may include modifiers, cursed or doused players, players who are holding a bomb or who are blackmailed etc. 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Sabotage Options

|               Name                     |                                              Description                                                         |     Type     |  Default  |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | :----------: | :-------: |
| Disable Sabotages                      | Disables Impostor's ability to use certain sabotages.                                                            |    Toggle    |    OFF    |
| ┣ Disable Reactor                      | Disables Impostor's ability to sabotage Reactor (Skeld, Mira HQ, Airship).                                       |    Toggle    |    OFF    |
| ┣ Disable Oxygen                       | Disables Impostor's ability to sabotage Oxygen (Skeld and Mira HQ).                                              |    Toggle    |    OFF    |
| ┣ Disable Lights                       | Disables Impostor's ability to sabotage Lights.                                                                  |    Toggle    |    OFF    | 
| ┣ Disable Communications               | Disables Impostor's ability to sabotage Communications.                                                          |    Toggle    |    OFF    |
| ┣ Disable Doors                        | Disables Impostor's ability to close Doors.                                                                      |    Toggle    |    OFF    |
| ┗ Disable Crash Course                 | Disables Impostor's ability to sabotage Crash Course (Airship only).                                             |    Toggle    |    OFF    |
| Skeld Reactor Countdown                | Customizes Countdown to fix Reactor on Skeld before death.                                                       |     Time     |  DEFAULT  | 
| Skeld Oxygen Countdown                 | Customizes Countdown to fix Oxygen on Skeld before death.                                                        |     Time     |  DEFAULT  | 
| Mira Reactor Countdown                 | Customizes Countdown to fix Reactor on Mira HQ before death.                                                     |     Time     |  DEFAULT  | 
| Mira Oxygen Countdown                  | Customizes Countdown to fix Oxygen on Mira HQ before death.                                                      |     Time     |  DEFAULT  | 
| Polus Reactor Countdown                | Customizes Countdown to fix Reactor on Polus before death.                                                       |     Time     |  DEFAULT  | 
| Airship Crash Course Countdown         | Customizes Countdown to fix Crash Course on Airship before death.                                                |     Time     |  DEFAULT  | 


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mayhem Options

|               Name                     |                                              Description                                                         |     Type     |  Default  |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | :----------: | :-------: |
| Enable Random Maps                     | Randomizes which map is used to play each game.                                                                  |    Toggle    |    OFF    |
| ┣ Skeld                                | Allows for Skeld to be included in the list of randomized maps.                                                  |    Toggle    |    OFF    |
| ┣ Mira                                 | Allows for Mira HQ to be included in the list of randomized maps.                                                |    Toggle    |    OFF    |
| ┣ Polus                                | Allows for Polus to be included in the list of randomized maps.                                                  |    Toggle    |    OFF    |
| ┗ Airship                              | Allows for Airship to be included in the list of randomized maps.                                                |    Toggle    |    OFF    |
| Random Spawn                           | Makes player spawn in random places around the map instead of everyone spawning in the same spot.                |    Toggle    |    OFF    |
| Camo Comms                             | Makes all players look the same (same color and removes outfits) when Communications are sabotaged.              |    Toggle    |    OFF    |
| All Roles Can Vent                     | Gives all roles the ability to vent.                                                                             |    Toggle    |    OFF    |


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Miscellaneous Options

|               Name                     |                                              Description                                                         |     Type     |  Default  |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | :----------: | :-------: |
| Assigned Pet                           | Chooses what pet will be assigned to people who do not have a pet.*                                              |    Options   |   RANDOM  |
| Allow /name                            | Allows players (choose between friends only, or everyone) to change their name using /name.                      |    Toggle    |    OFF    |
| Allow /color and /level                | Allows players (choose between friends only, or everyone) to change thier color or level using /color and /level |    Toggle    |    OFF    | 
| Auto Display Results                   | Automatically displays the results of the last game after the game ends.                                         |    Toggle    |    ON     |
| Color Names                            | Displays everyone's name as the color of their Among Us character.                                               |    Toggle    |    OFF    |
| Ladder Death                           | Chance of falling from a ladder and dying (Airship Only).                                                        |  Percentage  |    OFF    | 

*Many roles require a pet in order to function. The game will automatically assign a pet to any players who don't have one. 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Roles

| Impostor                               | Crewmate                        | Neutral Killing                   | Neutral Passive                        | Modifier                  |
| -------------------------------------- | ------------------------------- | --------------------------------- | -------------------------------------- | ------------------------- |
| [Blackmailer](#blackmailer)            | [Alchemist](#alchemist)         | [Agitater](#agitater)             | [Amnesiac](#amnesiac)                  | [Bait](#bait)             |
| [Bounty Hunter](#bounty-hunter)        | [Bastion](#bastion)             | [Arsonist](#arsonist)             | [Archangel](#archangel)                | [Bewilder](#bewilder)     |
| [Camouflager](#camouflager)            | [Bodyguard](#bodyguard)         | [Blood Knight](#blood-knight)     | [Copy-Cat](#copy-cat)                  | [Bloodlust](#bloodlust)   |
| [Conman](#conman)                      | [Chameleon](#chameleon)         | [Demon](#demon)                   | [Executioner](#executioner)            | [Deadly](#deadly)         |
| [Consort](#consort)                    | [Charmer](#charmer)             | [Egoist](#egoist)                 | [Hacker](#hacker)                      | [Diseased](#diseased)     |
| [Creeper](#creeper)                    | [Crusader](#crusader)           | [Hitman](#hitman)                 | [Jester](#jester)                      | [Flash](#flash)           |
| [Disperser](#disperser)                | [Demolitionist](#demolitionist) | [Jackal](#jackal)                 | [Opportunist](#opportunist)            | [Nimble](#nimble)         |
| [Escapist](#escapist)                  | [Dictator](#dictator)           | [Juggernaut](#juggernaut)         | [Phantom](#phantom)                    | [Oblivious](#oblivious)   |
| [FireWorker](#fireworker)              | [Doctor](#doctor)               | [Marksman](#marksman)             | [Postman](#postman)                    | [Romantic](#romantic)     |
| [Freezer](#freezer)                    | [Escort](#escort)               | [Necromancer](#necromancer)       | [Schrodinger's Cat](#schrodingers-cat) | [Sleuth](#sleuth)         |
| [Grenadier](#grenadier)                | [Ex-Convict](#ex-convict)       | [Occultist](#occultist)           | [Survivor](#survivor)                  | [Tiebreaker](#tiebreaker) |
| [Identity Thief](#identity-thief)      | [Herbalist](#herbalist)         | [Pelican](#pelican)               | [Terrorist](#terrorist)                | [Torch](#torch)           |
| [Janitor](#janitor)                    | [Investigator](#investigator)   | [Retributionist](#retributionist) |                                        | [Watcher](#watcher)       |
| [Mafioso](#mafioso)                    | [Mayor](#mayor)                 | [The Glitch](#the-glitch)         |                                        | [Workhorse](#workhorse)   |
| [Mare](#mare)                          | [Mechanic](#mechanic)           | [Werewolf](#werewolf)             |                                        |                           |
| [Mastermind](#mastermind)              | [Medic](#medic)                 |                                   |                                        |                           |
| [Miner](#miner)                        | [Medium](#medium)               |                                   |                                        |                           |
| [Morphling](#morphling)                | [Mystic](#mystic)               |                                   |                                        |                           |
| [Ninja](#ninja)                        | [Observer](#observer)           |                                   |                                        |                           |
| [Pickpocket](#pickpocket)              | [Oracle](#oracle)               |                                   |                                        |                           |
| [Puppeteer](#puppeteer)                | [Physicist](#physicist)         |                                   |                                        |                           |
| [Serial Killer](#serial-killer)        | [Psychic](#psychic)             |                                   |                                        |                           |
| [Sniper](#sniper)                      | [Repairman](#repairman)         |                                   |                                        |                           |
| [Swooper](#swooper)                    | [Sheriff](#sheriff)             |                                   |                                        |                           |
| [Time Thief](#time-thief)              | [Snitch](#snitch)               |                                   |                                        |                           |
| [Vampire](#vampire)                    | [Speedrunner](#speedrunner)     |                                   |                                        |                           |
| [Warlock](#warlock)                    | [Swapper](#swapper)             |                                   |                                        |                           |
| [Witch](#witch)                        | [Tracker](#tracker)             |                                   |                                        |                           |
| [Yin Yanger](#yin-yanger)              | [Transporter](#transporter)     |                                   |                                        |                           |
|                                        | [Trapster](#trapster)           |                                   |                                        |                           |
| [Crewposter (Madmate)](#crewposter)    | [Veteran](#veteran)             |                                   |                                        |                           |
| [Mad Guardian (Madmate)](#madguardian) | [Vigilante](#vigilante)         |                                   |                                        |                           |
| [Madmate (Madmate)](#madmate)          |                                 |                                   |                                        |                           |
| [Mad Snitch (Madmate)](#madsnitch)     |                                 |                                   |                                        |                           |
| [Parasite (MadMate)](#parasite)        |                                 |                                   |                                        |                           |




# Host Only Roles

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## GM

The GM (Game Master) is an observer role.<br>
Their presence has no effect on the game itself, and all players know who the GM is at all times.<br>
Always assigned to a host and is ghosted from the start.<br>

# Impostors

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Blackmailer 

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Blackmail A Player<br>
__Indicator/Symbols__: "BLACKMAILED" Text Over Targeted Player<br>

#### Role Description

Shapeshift into a player to blackmail them.<br>
During meeting, the blackmailed player will have text displaying "BLACKMAILED" to all players.<br>
If the player writes a certain number of messages (determined by host) while blackmailed, they will be executed.<br>

### Game Options
|               Name                    |                                  Description                              |     Type     |  Default  | 
| ------------------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Blackmailer                           | The probability of the Blackmailer appearing                              |  Percentage  |    0%     |
| Maximum                               | How many Blackmailers should spawn                                        |    Number    |     1     |
| Warnings Until Death                  | How many warnings the Blackmailed player gets before suicide              |    Number    |     0     |
| Show Blackmailed To All               | Show the 'BLACKMAILED' indicator to all players                           |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Bounty Hunter

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Reduced Kill Cooldown<br>
__Indicatior/Symbols__: Text Indicator Displaying Current Target<br>

`Originally Developed by: Discussions`<br>
`Idea by The Other Roles`<br>

#### Role Description 
Collect Bounty from Target players (marked by black name).<br>
If the Bounty Hunter kills their target, their kill cooldown is significantly reduced for their next kill.<br>
The time it takes for the target to change, the kill cooldown after killing their target, and kill cooldown after killing a non-target are predetermined by host in settings.<br>

### Game Options
|               Name                    |                                  Description                              |     Type     |  Default  | 
| ------------------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| BountyHunter                          | The probability of the BountyHunter appearing                             |  Percentage  |    0%     |
| Maximum                               | How many BountyHunters should spawn                                       |    Number    |     1     |
| Time Until New Target                 | Time before the BountyHunters target is changed                           |     Time     |    60     |
| Kill Cooldown After Killing Target    | The cooldown of the BountyHunter's Kill button after killing their target |     Time     |    15     |
| Kill Cooldown After Killing Other     | The cooldown of the BountyHunter's Kill button after killing a non-target |     Time     |   37.5    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Camouflager

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Shapeshifter<br>
__Ability__: Disguise Everyone<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: こう。`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
Shapeshift into a player and cause every living player to shapeshift into the chosen player for a short amount of time.<br>
When the duration is over, or if a meeting is called, players return to their normal form.<br>

### Game Options
|       Name           |                  Description                        |     Type     |  Default  | 
| -------------------- | --------------------------------------------------- | :----------: | :-------: |
| Camouflager          | The probability of the Camouflager appearing        |  Percentage  |    0%     |
| Maximum              | How many Camouflagers should spawn                  |    Number    |     1     |
| Camouflage Cooldown  | The cooldown of the Camouflager's Shapeshift button |     Time     |   17.5s   |
| Camouflage Duration  | Amount of time players are shifted for              |     Time     |   17.5s   |
| Can Vent             | Whether the Camouflager has a Vent button or not    |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Conman

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Sabotage Meetings<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by yoclobo (Manipulator)`<br>

#### Role Description
Reporting a body killed by the Conman will sabotage the meeting.<br>
The Anonymous Voting option may be toggled (if you had this on, it is now off and vice versa) & Voting/Discussion Time will be decreased (amount predetermined by host in settings).<br>
The Conman’s voting and discussion time overwrites the ones of TimeThief.<br>
The Conman also has options for a separate Kill-Cooldown.<br>

### Game Options
|            Name           |                      Description                   |     Type     | Default | 
| ------------------------- | -------------------------------------------------- | :----------: | :-----: |
| Conman                    | The probability of the Conman appearing            |  Percentage  |   0%    |
| Maximum                   | How many Conmans should spawn                      |    Number    |    1    |
| Kill Cooldown             | The cooldown of the Conman's Kill button           |     Time     | Global  |
| Discussion Time Decrease  | The amount of time removed from Discussion Time    |     Time     |   30s   |
| Voting Time Decrease      | The amount of time removed from Voting Time        |     Time     |   15s   |
| Affect Anonymous Voting   | Whether the Conman's kills affect Anonymous Voting |    Toggle    |   ON    |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Consort 

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Roleblock Players<br>
__Indicatior/Symbols__: Text Indicator Displaying Current Mode<br>

`Originally Developed by: Discussions`<br>
`Idea by Det`<br>

#### Role Description
Use the Pet button to alternate between Role-Blocking and Killing. <br>
Role-Blocks prevent killing, reporting dead bodies, calling meetings, shapeshifting, and venting.<br>

### Game Options
|        Name             |                      Description                  |     Type     |    Default    | 
| ----------------------- | ------------------------------------------------- | :----------: | :-----------: | 
| Consort                 | The probability of the Consort appearing          |  Percentage  |      0%       |
| Maximum                 | How many Consorts should spawn                    |    Number    |       1       |
| Roleblock Cooldown      | The cooldown of the Consort's Kill button         |     Time     |      45s      |
| Roleblock Duration      | The duration of the Consort's Role-Block function |    Number    | Until Meeting |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Creeper

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Mass Distruction<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Discussions`<br>

#### Role Description
The Creeper's only job is to cause as much devasation as possible.<br>
Use either your Pet or Shapeshift button to kill yourself and any player within a radius.<br>
You might find yourself lucky and be protected from your bombs with a shield (ex. medic shield) and live to see another day. If the option is off however, not even the medic shield will protect you.<br>

### Game Options
|        Name        |                               Description                               |     Type     |    Default    | 
| ------------------ | ----------------------------------------------------------------------- | :----------: | :-----------: |
| Creeper            | The probability of the Creeper appearing                                |  Percentage  |      0%       |
| Maximum            | How many Creepers should spawn                                          |    Number    |       1       |
| Can Kill Normally  | Whether the Creeper can kill normally                                   |    Toggle    |      ON       |
| Can Be Shielded    | Allows Creeper to be shielded by other players                          |    Toggle    |      ON       |
| Explosion Radius   | The radius at which players will be affected by the Creeper's explosion |    Toggle    |     Small     |
| Grace Period       | The amount of time before self explosion                                |     Time     |      10s      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Disperser 

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Teleport Players<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
Use Pet button to teleport everyone to a random vent.<br>

### Game Options
|           Name           |                         Description                       |     Type     |  Default  | 
| ------------------------ | --------------------------------------------------------- | :----------: | :-------: |
| Disperser                | The probability of the Disperser appearing                |  Percentage  |    0%     |
| Maximum                  | How many Dispersers should spawn                          |    Number    |     1     |
| Disperse Cooldown        | The cooldown of the Disperser's Pet Button                |     Time     |   12.5s   | 
| Disperser Gets Dispersed | Whether Disperser is teleported when ability is activated |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Escapist

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Shapeshifter<br>
__Ability__: Mark A Location & Strategically Escape<br>
__Indicatior/Symbols__: Text Cooldown Displaying Time Until Able To Escape & Until Next Mark<br>

`Originally Developed by: Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
First use Pet button to mark a location. Then, after a set cooldown, you can re-use the Pet button to teleport back to your marked location.<br> 
This will then put the mark ability back on cooldown.<br>

### Game Options
|           Name           |                      Description                      |     Type     |  Default  | 
| ------------------------ | ----------------------------------------------------- | :----------: | :-------: |
| Escapist                 | The probability of the Escapist appearing             |  Percentage  |    0%     |
| Maximum                  | How many Escapists should spawn                       |    Number    |     1     |
| Cooldown After Mark      | The cooldown of the Escapist's Mark ability           |     Time     |    5s     | 
| Cooldown After Escape    | The cooldown of the Escapist's Escape ability         |     Time     |    40s    |
| Clear Mark After Meeting | This option removes the Escapist's Mark after meeting |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## FireWorker

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter<br>
__Ability__: Explode Players Within Radius<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: こう。`<br>
`Idea by こう。`<br>

#### Role Description
Use Pet button to plant a fireworks (i.e. bombs) around the map until Max Firework Count has been reached.<br>
Make sure you have enough room for the pet animation.<br>
Shapeshift to detonate all of the Fireworks, killing everyone within radius of each one.<br>
Note: The explosion goes through walls.<br>
The FireWorker can aslo kill normally between placing fireworks.<br>

### Game Options
|              Name               |                                                Description                                                |      Type      |  Default   | 
| ------------------------------- | --------------------------------------------------------------------------------------------------------- | :------------: | :--------: |
| Fireworker                      | The probability of the FireWorkers appearing                                                              |   Percentage   |     0%     |
| Maximum                         | How many FireWorkers should spawn                                                                         |     Number     |      1     |
| Total Firework Count            | How many fireworks can be placed on the map                                                               |     Number     |      3     |
| Fireworks Per Round             | How many fireworks can be placed per round                                                                |  Number/Limit  |  No Limit  |
| ┗ Fireworks Ability Cooldown    | The cooldown of the Fireworker's ability to plant fireworks (bombs)                                       |      Time      |     20s    |
| Firework Explosion Radius       | The Distance a player can be from a Firework and be affected by it's explosion                            |      Number    |     0.8    |
| Firework Delay                  | The amount of time it takes from shapeshift for the fireworks to explode                                  |      Time      |     1s     |
| ┗ Warn Players Before Explosion | All players within radius get a reactor alarm and text letting them know the firework is about to explode |     Toggle     |     ON     |
| Must Be Last Impostor           | Whether the Fireworker can detonate fireworks before they are Last Impostor                               |     Toggle     |     ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Freezer 

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter<br>
__Ability__: Shapeshift Into A Player To Freeze Them In Place<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Discussions`<br>

#### Role Description
The Freezer can freeze a player in place by shapeshifting into them.<br>
The player will be frozen until the Freezer unshapeshifts.<br>
Freezer may kill normally shifted or unshifted.<br>

### Game Options
|      Name       |                    Description                  |     Type     |  Default  | 
| --------------- | ----------------------------------------------- | :----------: | :-------: |
| Freezer         | The probability of the Freezer appearing        |  Percentage  |    0%     |
| Maximum         | How many Freezers should spawn                  |    Number    |     1     |
| Freeze Cooldown | The cooldown of the Freezer's Shapeshift Button |     Time     |    20     |
| Freeze Duration | Amount of time that the player is frozen for    |     Time     |    10     |
| Can Vent        | Whether Freezer can vent or not                 |    Toggle    |    ON     | 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Grenadier

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Blind Nearby Players<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Using the Pet button sets off a bomb, blinding players in a fixed-distance.<br>
It may also blind allied-Impostors, based on host's settings.<br>
During this time The Grenadier may kill undetected.<br>

### Game Options
|        Name         |                     Description                        |     Type     |  Default  | 
| ------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Grenadier           | The probability of the Grenadier appearing             |  Percentage  |    0%     |
| Maximum             | How many Grenadiers should spawn                       |    Number    |     1     |
| Amount of Grenades  | How many grenades are granted to the Grenadier         |    Number    |     3     |
| Blind Cooldown      | The cooldown of the Grenadier's Pet button             |     Time     |    30s    |
| Blind Duration      | The amount of time that lights are out                 |     Time     |    15s    |
| Blind Effect Radius | The radius of which players are affected by lights out |    Number    |    1.8    |
| Can Blind Allies    | Whether Grenadier can blind allies or not              |    Toggle    |    OFF    |
| Can Vent            | Whether Grenadier has a vent button or not             |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Identity Thief

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Shapeshifter<br>
__Ability__: Shapeshift Into Your Victim<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by paigecourtney "CC"`<br>

#### Role Description
The Identity Thief shifts into whoever they kill.<br>
The disguise lasts until they are ready to kill again, or, optionally, until they kill another player and shift into their next victim.<br>

### Game Options  
|          Name           |                            Description                          |     Type     |  Default  | 
| ----------------------- | --------------------------------------------------------------- | :----------: | :-------: |
| Identity Thief          | The probability of the Identity Thief appearing                 |  Percentage  |    0%     |
| Maximum                 | How many Identity Thieves should spawn                          |    Number    |     1     |
| Disguise Settings       | Options for how long the Identity Thief stays disguised for     |    Toggle    |  Kill CD  |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Janitor 

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Clean Bodies With Report Button<br>
__Indicatior/Symbols__: None<br>

`Idea by Town of Us Reactivated`

#### Role Description
Choose between killing and cleaning at the end of kill cooldown.<br>
Once the choice is made, the Janitor's Kill Button is reset.<br>
Use Report button to clean dead bodies, making them unreportable.<br>
Use Kill button to kill players<br>

### Game Options (incomplete)
|            Name            |                    Description                      |     Type     |  Default  | 
| -------------------------- | --------------------------------------------------- | :----------: | :-------: |
| Janitor                    | The probability of the Janitor appearing            |  Percentage  |    0%     |
| Maximum                    | How many Janitors should spawn                      |    Number    |     1     |
| Clean On Kill              | Whether Janitor cleans bodies when they kill or not |    Toggle    |    ON     |
| ┗ Kill Cooldown Multiplier | Multiplier required when Clean On Kill is ON        |  Multiplier  |   1.5x    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mafioso

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Engineer<br>
__Ability__: Gain Cash By Completing Tasks<br>
__Indicatior/Symbols__: Counter Showing Number of Bullets (striked-through until a gun is achieved) AND Cash Counter<br>

#### Role Description
The Mafioso is a unique impostor role, who cannot kill off the bat. Instead the Mafioso must complete tasks in order to gain cash. During meetings, the Mafioso can use their cash to purchase a couple of different items.<br>
Type /o to see how much each item costs.<br> 
Only items you are able to use/buy will show up in the shop.<br>

__Tommy Gun__: Allows the Mafioso to kill (one time purchase)<br>
__Bullet__: Required to use with the Tommy Gun<br>
__Bulletproof Vest__: Gives the Mafioso one-time use invincibility for next round<br>
__Role Revealer__: Allows the Mafioso to reveal the role of one other player<br>

### Game Options
|               Name              |               Description                |     Type     |  Default  |
| ------------------------------- | ---------------------------------------- | :----------: | :-------: |
| Mafioso                         | The probability of the Mafioso appearing |  Percentage  |    0%     |
| Maximum                         | How many Mafiosos should spawn           |    Number    |     1     |
| Modify Shop Costs               | Allows for custom costs for Mafioso Shop |    Toggle    |    OFF    |
| ┣ Gun Cost                      | The custom cost of the Tommy Gun         |    Number    |     6     |
| ┣ Bullet Cost                   | The custom cost of the bullet            |    Number    |     6     |
| ┣ Vest Cost                     | The custom cost of the bulletproof vest  |    Number    |     6     |
| ┗ Role Revealer Cost            | The custom cost of the Role Revealer     |    Number    |     5     |
| Starts Game With Gun            | Whether Mafioso starts with a gun or not |    Toggle    |    OFF    |
| Gun Cooldown                    | The cooldown of the Mafioso's Tommy Gun  |    Number    |  Global   |
| Cash From Reporting Bodies      | Cash received for reporting bodies       |    Number    |     2     |
| Refresh Tasks When All Complete | Allows more tasks for Mafioso            |    Toggle    |    ON     |

_The Global option for Gun Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mare

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Buffed During Sabotage<br>
__Indicatior/Symbols__: If Enabled, Your Name Will be Purple During Your Ability<br>

`Originally Developed by: Kihi, しゅー, そうくん, ゆりの`<br>
`Idea by Kihi`<br>

#### Role Description
Mare gains special powers during specific sabotages (determined by host). These powers may include: Increased Speed and Decreased Kill-Cooldown.<br>
Be careful! If enabled in settings, your name will appear Purple while your ability is active.

### Game Options
|               Name             |                                 Description                                    |    Type    |    Default    |
| ------------------------------ | ------------------------------------------------------------------------------ | :--------: | :-----------: |
| Mare                           | The probability of the Mare appearing                                          | Percentage |      0%       | 
| Maximum                        | How many Mares should spawn                                                    |  Number    |       1       |
| Speed Modifier During Sabotage | Controls speed boost during sabotages                                          |  Number    |     1.5x      |
| Can Kill Without Sabotage      | Whether Mare can kill when there isn't a sabotage                              |  Toggle    |      ON       |
| ┗ Normal Kill Cooldown         | Mare's normal Kill cooldown                                                    |   Time     |     30s       |
| Colored Name During Sabotage   | Whether Mare's name is colored during sabotage                                 |  Toggle    |      ON       |
| Kill Cooldown During Sabotage  | Mare's Kill cooldown during a sabotage                                         |   Time     |     15s       |
| Specific Sabotage Settings     | Whether Mare's ability can be used during lights only or individual sabotages  |  Toggle    |  Lights Only  |
| ┣ Lights                       | Whether Mare can use it's ability during Lights sabotage (All Maps)            |  Toggle    |      ON       |
| ┣ Communications               | Whether Mare can use it's ability during Communications sabotage (All Maps)    |  Toggle    |      OFF      |
| ┣ Oxygen                       | Whether Mare can use it's ability during Oxygen sabotage (The Skeld & MIRA HQ) |  Toggle    |      OFF      |
| ┣ Reactor                      | Whether Mare can use it's ability during Reactor sabotage (All Maps)           |  Toggle    |      OFF      |
| ┗ Crash Course                 | Whether Mare can use it's ability during Avert Crash Course sabotage (Airship) |  Toggle    |      OFF      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mastermind 

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Sabotage Meetings<br>
__Indicatior/Symbols__: "Manipulated!" text on manipulated players<br>

#### Role Description
Mastermind marks a player with their Kill button. After a delay, that player will gain text saying they've been Manipulated, and a countdown will begin.<br> 
That player must kill another player before their countdown ends (by using either Pet or Kill), otherwise they suicide.

### Game Options
|              Name             |                   Description                    |     Type     |  Default  |
| ----------------------------- | ------------------------------------------------ | :----------: | :-------: |
| Mastermind                    | The probability of the Mastermind appearing      |  Percentage  |    0%     |
| Maximum                       | How many Masterminds should spawn                |    Number    |     1     |
| Manipulation Cooldown         | The cooldown of the Manipulator's Kill button    |    Number    |  Global   |
| Manipulated Player Limit      | How many players can be manipulated              |    Number    |     ∞     |
| Impostors Can See Manipulated | Whether Impostors can see manipulated players    |    Toggle    |    ON     |
| Time Until Suicide            | How much time the manipulated player has to kill |     Time     |   12.5s   |

_The Global option for Manipulation Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Miner

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Teleportation<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
Use the Pet button to teleport to the last vent used.<br>
Make sure you have enough room for the pet animation.<br>
Kill, vent, and sabotage like any other impostor role.<br>

### Game Options
|           Name         |                   Description                     |     Type     |  Default  | 
| ---------------------- | ------------------------------------------------- | :----------: | :-------: |
| Miner                  | The probability of the Miner appearing            |  Percentage  |    0%     |
| Maximum                | How many Miners should spawn                      |    Number    |     1     |
| Miner Ability Cooldown | The cooldown on the Miner's teleportation ability |     Time     |   17.5s   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Morphling

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter<br>
__Ability__: Can Morph Into Other Players<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Innersloth`<br>

#### Role Description 
The Morphling can shapeshift themselves into any player that was still alive at the end of the last meeting.<br>
It is a renamed Shapeshifter role in vanilla Among Us.<br>

### Game Options
|         Name        |                     Description                       |     Type     |  Default  | 
| ------------------- | ----------------------------------------------------- | :----------: | :-------: |
| Morphling           | The probability of the Morphling appearing            |  Percentage  |    0%     |
| Maximum             | How many Morphlings should spawn                      |    Number    |     1     |
| Shapeshift Cooldown | The cooldown of the Morphling's Shapeshift button     |     Time     |    30s    |
| Shapeshift Duration | The amount of time the Morphling can stay shifted for |     Time     |    15s    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Ninja

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter or Impostor<br>
__Ability__: Teleportation<br>
__Indicatior/Symbols__: Text indicator Displaying Current Mode<br>

`Originally Developed by: Discussions`<br>
`Idea by The Other Roles`<br>

#### Ninja Ability Activation: Shapeshift Button
Use Kill Button while shifted to mark target.<br>
When the Ninja unshifts, they will be teleported to their target and complete the kill.<br>
Use Kill Button while unshifted to kill normally.<br>
Shapeshift duration and cooldown is infinite.<br>

#### Ninja Ability Activation: Pet Button
Use Pet Button to mark target.<br>
Use Pet Button again to teleport to the target and execute the kill.<br>
Make sure you have enough room for the pet animation.<br>
Use Kill Button like normal if you haven't used the Pet Button to mark a target yet.<br>

#### Players Teleport to Ninja
With this option the Ninja no longer teleports to the target.<br>
Instead, the target is teleported to the Ninja where the kill will be executed.<br>


### Game Options 
|           Name            |                     Description                         |    Type    |  Default   | 
| ------------------------- | ------------------------------------------------------- | :--------: | :--------: |
| Ninja                     | The probability of the Ninja appearing                  | Percentage |    0%      |
| Maximum                   | How many Ninjas should spawn                            |   Number   |     1      |
| Players Teleport to Ninja | Allows marked players to teleport to Ninja              |   Toggle   |    OFF     |
| Ninja Ability Activation  | Whether the Ninja uses Shapeshift or Pet to mark target |   Toggle   | Pet Button |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Pickpocket

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Steals Votes From Their Kills <br>
__Indicatior/Symbols__: Counter Displaying Current Vote Increase<br>

`Originally Developed by: Discussions`<br>
`Idea by Discussions`<br>

#### Role Description
The Pickpocket is an Impostor who steals the votes of players they kill.<br>
These votes stack up, which can make the Pickpocket very powerful.<br>

### Game Options
|             Name            |                         Description                          |    Type    |  Default   | 
| --------------------------- | ------------------------------------------------------------ | :--------: | :--------: |
| Pickpocket                  | The probability of the Pickpocket appearing                  | Percentage |    0%      |
| Maximum                     | How many Pickpockets should spawn                            |   Number   |     1      |
| Kill Cooldown               | The cooldown of the Pickpocket's Kill button                 |    Time    |   Global   |
| Maximum Additional Votes    | The maximum amount of extra votes the Pickpocket can acquire |   Number   |     5      |
| Resets Votes After Meetings | Whether Pickpocket loses votes after meeting                 |   Toggle   |    ON      |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Puppeteer

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Control Players<br>
__Indicatior/Symbols__: "◆" Indicator On Puppeted Players<br>

`Originally Developed by: Discussions`<br>
`Idea by The Other Roles`<br>

#### Role Description
The Puppeteer can control a player and force them to kill the next non-impostor they come near.<br>
Use the Kill button next to a player to gain control over them.<br>
If the killed player has an ability that activates upon death, the effect will land on the controlled player instead of the Puppeteer.<br>
It is not possible for puppeteer to perform a normal kill.<br>

### Game Options 
|   Name    |                Description                 |    Type    |  Default   | 
| --------- | ------------------------------------------ | :--------: | :--------: |
| Puppeteer | The probability of the Puppeteer appearing | Percentage |    0%      |
| Maximum   | How many Puppeteers should spawn           |   Number   |     1      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Serial Killer 

<img align="right" width="" height="300" src="">

__Faction__: Impostors <br>
__Base__: Impostor<br>
__Ability__: The Impostor's Groupie
__Indicatior/Symbols__: Timer Showing When Serial Killer Is Going To Suicide<br>

`Originally Developed by: Town of Host`<br>
`Idea by Town of Host`<br>

#### Role Description
Has a reduced Kill-Cooldown (determined by host). Kill players before cooldown expires to avoid suicide.

### Game Options
|              Name             |                        Description                       |    Type    |  Default   | 
| ----------------------------- | -------------------------------------------------------- | :--------: | :--------: |
| Serial Killer                 | The probability of the Serial Killer appearing           | Percentage |    0%      |
| Maximum                       | How many Serial Killers should spawn                     |   Number   |     1      |
| Kill Cooldown                 | Cooldown of the Serial Killer's Kill button              |    Time    |   7.5s     |
| Time Until Suicide            | Amount of time given to the Serial Killer to make a kill |    Time    |    80s     |
| Timer Begins After First Kill | Whether the Suicide Timer begins after the first kill    |   Toggle   |    OFF     | 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Sniper

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter<br>
__Ability__: Can Kill From A Far Distance<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: こう。`<br>
`Idea by Nebula on the Ship`<br>

#### Normal Sniper Mode
Use Shapeshift button to shift into another player.<br>
Take 1-2 steps in the direction you want to fire.<br>
Unshift to shoot. A bullet will travel in that direction until it kills a player.<br>
When out of bullets, Sniper turns to normal impostor role.<br>

#### Load Bullet Mode
Use Pet Button to load a bullet and get ready to shoot.<br>
Make sure you have enough room to use your pet button.<br>
To shoot, the Sniper must take a few steps in the direction they aim to shoot, and then shapeshift.<br>

### Game Options
|          Name          |                         Description                              |    Type    |      Default       | 
| ---------------------- | ---------------------------------------------------------------- | :--------: | :----------------: |
| Sniper                 | The probability of the Sniper appearing                          | Percentage |         0%         |
| Maximum                | How many Snipers should spawn                                    |   Number   |         1          |
| Sniper Bullet Count    | How many bullets the sniper can shoot                            |   Number   |         26         |
| Precise Shooting       | View Precise shooting diagram below                              |   Toggle   |         ON         |
| Can Be Vetted on Snipe | The Sniper is affected by the Veteran's ability when using Snipe |   Toggle   |         ON         |
| Sniper Mode            | Whether Sniper uses Normal Sniper Mode or Loaded Bullet Mode     |   Toggle   | Normal Sniper Mode |
| ┣ Load Bullet Cooldown | The cooldown between loading bullets                             |    Time    |        17.5        | 
| ┗ Max Loaded Bullets   | How many bullets you may load in one round                       |   Number   |          1         |

#### Precise Shooting: OFF<BR>
![off](https://cdn.discordapp.com/attachments/1028575028092084315/1061378165974515752/Untitled155_20230108014453.png)<BR>
#### Precise Shooting: ON<BR>
![on](https://cdn.discordapp.com/attachments/1028575028092084315/1061378166402318426/Untitled155_20230108014306.png)<BR>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Swooper

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__: Impostor<br>
__Ability__: Invisibility<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
A normal impostor that can go invisible when entering a vent. While invisible, the Swooper can do all normal things (kill, sabotage, vent).<br>
Be careful! Depending on the host's options you may be revealed when killing another player.<br>

### Game Options 
|               Name            |                         Description                              |    Type    | Default | 
| ----------------------------- | ---------------------------------------------------------------- | :--------: | :-----: |
| Sniper                        | The probability of the Swooper appearing                         | Percentage |    0%   |
| Maximum                       | How many Swoopers should spawn                                   |   Number   |    6    |
| Invisibility Cooldown         | The cooldown for the Swooper's Vent Button                       |    Time    |   45s   |
| Swooping Duration             | How long the Swooper can be invisible for                        |    Time    |   10s   |
| Can Be Seen By Allies         | Whether Swooper can be seen by other Impostors                   |   Toggle   |    ON   |
| Can Vent During Cooldown      | Whether the Swooper can vent normally during cooldown or not     |   Toggle   |   OFF   |
| Remain Invisible On Kill      | Allows Swooper to remain invisible when they kill                |   Toggle   |    ON   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Time Thief

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Decrease Meeting and Voting Time<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: integral, しゅー, そうくん, ゆりの`<br>
`Idea by みぃー`<br>

#### Role Description
Killing a player decreases meeting/voting time.<br>
Option: When TimeThief is expelled or killed, time is restored back to normal.<br>

### Game Options
|              Name              |                              Description                                     |    Type    |  Default   | 
| ------------------------------ | ---------------------------------------------------------------------------- | :--------: | :--------: |
| Time Thief                     | The probability of the Time Thief appearing                                  | Percentage |     0%     |
| Maximum                        | How many Time Thieves should spawn                                           |   Number   |     1      |
| Meeting Time Stolen            | How much time is taken off the Meeting Time per kill                         |    Time    |    25s     |
| Minimum Voting Time            | The lowest amount of time the voting duration can be lowered to.             |    Time    |    15s     |
| Return Stolen Time After Death | Whether the meeting/voting time is reverted to original when Time Thief dies |   Toggle   |     ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Vampire

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Delayed Kills<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Town of Host`<br>
`Idea by The Other Roles`<br>

#### Role Description
The Vampire bites it's targets, resulting in a delayed kill.<br>
The bitten player will die after several seconds or when the next meeting is called.<br>
If the vampire bites [Bait](#Bait), the player will die immediately and a self-report will be forced.<br>

### Vampiress 

<img align="right" width="" height="300" src="">

__Faction__: Impostor<br>
__Base__ Impostor<br>
__Ability__: Delayed & Normal Kills<br>
__Indicatior/Symbols__: Text Indicator Showing Current Mode<br>

`Created by Discussions`<br>
`Original Idea by shiftyrose`<br>

#### Vampiress Role Description 
The Vampiress works exactly like the [Vampire](#vampire) with one exception, it can also make direct kills.<br>
Use the Pet Button to switch between Bites and Kills.<br>

### Game Options
|      Name       |                 Description                 |    Type    |  Default   | 
| --------------- | ------------------------------------------- | :--------: | :--------: |
| Vampire         | The probability of the Vampire appearing    | Percentage |    0%      |
| Maximum         | How many Vampires should spawn              |   Number   |     1      |
| Kill Delay      | The amount of time a kill is delayed        |    Time    |    7.5s    |
| Vampiress       | The probability of the Vampiress appearing  | Percentage |    0%      |
| ┣ Kill Cooldown | The cooldown of the Vampiress's Kill button |   Number   |   Global   |
| ┗ Kill Delay    | The amount of time a kill is delayed        |    Time    |    7.5s    |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Warlock

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Shapeshifter<br>
__Ability__: Can Curse Players<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by The Other Roles`<br>

#### Role Description
Use the Kill Button to curse a Player.<br>
The next time the Warlock shapeshifts, the cursed player will kill the nearest person.<br>
The Warlock may kill normally while shapeshifted.<br>
Be Careful! Cursed players can kill Impostors (and even the Warlock themself!).<br>

### Game Options
|              Name               |                Description               |    Type    |  Default   | 
| ------------------------------- | ---------------------------------------- | :--------: | :--------: |
| Warlock                         | The probability of the Warlock appearing | Percentage |    0%      |
| Maximum                         | How many Warlocks should spawn           |   Number   |     1      |
| Cursed Players Kill Immediately | Whether cursed players kill immediately  |   Toggle   |    ON      |
| ┗ Limited Cursed Kill Range     | Limits the cursed kill range             |   Toggle   |    OFF     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Witch

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Kill & Curse Players<br>
__Indicatior/Symbols__: Cross On Cursed Players <br>

`Originally Developed by: Town of Host`<br>
`Idea by The Other Roles`<br>

#### Role Description
Alternate between curses and killing by utilizing the Kill Button.<br>
Players who are cursed by the Witch will be seen with a cross during the meeting.<Br>
If the Witch is not voted off during this meeting, the cursed player dies.<br>
Regular kill self-reports [Bait](#Bait).<br>
Curse does not self-report [Bait](#Bait).<br>

### Game Options
|           Name            |                           Description                       |    Type    |  Default   | 
| ------------------------- | ----------------------------------------------------------- | :--------: | :--------: |
| Witch                     | The probability of the Witch appearing                      | Percentage |     0%     |
| Maximum                   | How many Witches should spawn                               |   Number   |     1      |
| Freely Switch Modes       | Use Pet Button to switch between Spells and Kills           |   Toggle   |     ON     |
| Switch Modes After Attack | Whether Kill/Curse mode automatically switches after attack |   Toggle   |     ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Yin Yanger

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Impostor<br>
__Ability__: Make Two Players Kill Each Other<br>
__Indicatior/Symbols__: None <br>

`Originally Developed by: Discussions`<br>
`Idea by Discussions`<br>

#### Role Description
The Yin Yanger is an Impostor with the ability to make two crewmates kill each other.<br>
Use the Kill button to tag two players. When they come within kill distance, they will kill each other.<br>
Yin Yanger can kill normally once targets have been set.<br>

### Game Options
|        Name       |                  Description                 |    Type    |  Default   | 
| ----------------- | -------------------------------------------- | :--------: | :--------: |
| Yin Yanger        | The probability of the Yin Yanger appearing  | Percentage |    0%      |
| Maximum           | How many Yin Yangers should spawn            |   Number   |     1      |
| Yin Yang Cooldown | The cooldown of the Yin Yanger's ability     |    Time    |   Global   |

_The Global option for Yin Yang Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Madmates 

## CrewPostor

<img align="right" width="" height="300" src="">

__Faction__: Neutral<br>
__Base__: Crewmate<br>
__Ability__: Kill Nearest Player By Finishing Tasks<br>
__Indicatior/Symbols__: None<br>
__Win Condition__: Win With Impostors<br>

`Originally Developed by: Discussions`<br>
`Idea by crewpostor`<br>

#### Role Description
Complete a task to instantly kill the player nearest you (even impostors and other killing roles).<br>

### Game Options
|              Name               |                         Description                         |     Type     |  Default  | 
| ------------------------------- | ----------------------------------------------------------- | :----------: | :-------: |
| CrewPostor                      | The probability of the CrewPostor appearing                 |  Percentage  |    0%     |
| Maximum                         | How many CrewPostors should spawn                           |    Number    |     1     |
| Warp To Target                  | Whether CrewPostor warps to target or kills without warping |    Toggle    |    ON     |
| Can Kill Allies                 | Whether Crewpostor can kill allies or not                   |    Toggle    |    OFF    |
| Refresh Tasks When All Complete | Allows more tasks for CrewPostor                            |    Toggle    |    ON     |
| Override CrewPostor's Tasks     | Allows the Host to add or remove tasks from CrewPostor      |    Toggle    |    OFF    |
| ┣ Allow Common Tasks            | Whether CrewPostor has Common Tasks or not                  |    Toggle    |    ON     |
| ┣ CrewPostor Long Tasks         | How many long tasks CrewPostor has                          |    Number    |     5     |
| ┗ CrewPostor Short Tasks        | How many short tasks CrewPostor has                         |    Number    |     6     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Madmate

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Engineer<br>
__Ability__: None (The Fallen Impostor)<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: Discussions`<br>
`Idea by libhalt`<br>

#### Role Description
The Madmate is a Impostor sided Crewmate. They are unable to kill and do not know who the Impostors are and the Impostors cannot tell them apart from other Crewmates.<br>

__What To Do:__<br>
Try to get back into the Impostors good graces.<br>
Act sus. Take suspicion off of Impostors by pretending to fix sabotages, venting, etc.<br>

### Game Options

|     Name     |              Description                 |     Type     |  Default  | 
| ------------ | ---------------------------------------- | :----------: | :-------: |
| Madmate      | The probability of the Madmate appearing |  Percentage  |    0%     |
| Maximum      | How many Madmates should spawn           |    Number    |     1     |
| Can Sabotage | Whether the Madmate can sabotage         |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mad Guardian

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Crewmate<br>
__Ability__: Finish Tasks To Become Unkillable<br>
__Indicatior/Symbols__: None<br>

`Originally Developed by: 空き瓶/EmptyBottle`<br>
`Idea by 空き瓶/EmptyBottle`<br>

### Role Description
The Mad Guardian is an Imposter sided Crewmate who has to do tasks to activate their ability. Madmates do not know who the Impostors are and the Impostors cannot tell who they are from other Crewmates.<br>

__What To Do:__<br>
Finish tasks to become immune from kills.<br>

### Game Options
|             Name              |                        Description                       |     Type     |  Default  | 
| ----------------------------- | -------------------------------------------------------- | :----------: | :-------: |
| MadGuardian                   | The probability of the MadGuardian appearing             |  Percentage  |    0%     |
| Maximum                       | How many MadGuardians should spawn                       |    Number    |     1     |
| Has Impostor Vision           | Whether Mad Guardian has Impostor vision                 |    Toggle    |    ON     |
| Can Vent                      | Whether Mad Guardian can vent                            |    Toggle    |    ON     |
| ┣ Vent Cooldown               | The cooldown of the Mad Guardian's Vent button           |     Time     |    20s    |
| ┗ Vent Duration               | The duration the Mad Guardian can stay in a vent         |     Time     |    9.5s   |
| Override Mad Guardian's Tasks | Allows the Host to add or remove tasks from Mad Guardian |    Toggle    |    OFF    | 
| ┣ Allow Common Tasks          | Whether the Mad Guardian has Common Tasks or not         |    Toggle    |    OFF    |
| ┣ Mad Guardian Long Tasks     | The amount of Long Tasks the Mad Guardian has            |    Number    |     5     |
| ┗ Mad Guardian Short Tasks    | The amount of Short Tasks the Mad Guardian has           |    Number    |     6     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mad Snitch

<img align="right" width="" height="300" src="">

__Faction__: Impostors<br>
__Base__: Crewmate or Engineer<br>
__Ability__: Finish Tasks To See Imps<br>
__Indicatior/Symbols__: None <br>

`Originally Developed by: そうくん`<br>
`Idea by そうくん`<br>

#### Role Description
The Mad Snitch is an Imposter sided Crewmate who has to do tasks to activate their ability. Much like the Snitch, The Mad Snitch must complete tasks to figure out the Imposters to defend them in meetings. They do not know who the Impostors are and the Impostors cannot tell them apart from other Crewmates.<br>

__What To Do:__<br>
Finish tasks to see who the Impostors are & defend them in meetings.<br>
Has the option to vent.<br>

### Game Options
|              Name           |                       Description                      |     Type     |  Default  | 
| --------------------------- | ------------------------------------------------------ | :----------: | :-------: | 
| Mad Snitch                  | The probability of the Mad Snitch appearing            |  Percentage  |    0%     |
| Maximum                     | How many Mad Snitches should spawn                     |    Number    |     1     |
| Has Impostor Vision         | Whether Mad Snitch has Impostor vision                 |    Toggle    |    ON     |
| Can Vent                    | Whether Mad Snitch can vent                            |    Toggle    |    ON     |
| ┣ Vent Cooldown             | The cooldown of the Mad Snitch's Vent button           |     Time     |    20s    |
| ┗ Vent Duration             | The duration the Mad Snitch can stay in a vent         |     Time     |    9.5s   | 
| Override Mad Snitch's Tasks | Allows the Host to add or remove tasks from Mad Snitch |    Toggle    |    OFF    | 
| ┣ Allow Common Tasks        | Whether the Mad Snitch has Common Tasks or not         |    Toggle    |    OFF    |
| ┣ Mad Snitch Long Tasks     | The amount of Long Tasks the Mad Snitch has            |    Number    |     3     |
| ┗ Mad Snitch Short Tasks    | The amount of Short Tasks the Mad Snitch has           |    Number    |     3     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Parasite

<img align="right" width="" height="300" src="">

__Faction__: Impostors (MadMates)<br>
__Base__: Shapeshifter<br>
__Ability__: Fallen Impostor (Buffed)<br>
__Indicatior/Symbols__:

`Originally Developed by: Discussions`<br>
`Idea by Loonie`<br>

#### Role Description
The Parasite is an Impostor Sided Killer who is able to kill but doesn't know who the Imposters are and vice versa. The Parasite is able to do everything that a regular imposter can do, and it must work with the Imposters to win together.. If they're still alive, that is. *wink*

### Game Options
|      Name     |                  Description                  |    Type    |  Default   | 
| ------------- | --------------------------------------------- | :--------: | :--------: |
| Parasite      | The probability of the Parasite appearing     | Percentage |    0%      |
| Maximum       | How many Parasite should spawn                |   Number   |     1      |
| Kill Cooldown | The cooldown of the Parasites Kill button     |   Number   |   Global   |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Crewmate

## Alchemist 

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Collect Ingredients & Create Potions<br>
__Indicator/Symbols__: <br><br>
_Ingredients_<br>
◆ = Catalyst (Source: Completing Tasks)<br>
Θ = Theta Rift (Source: Random Spawn)<br>
⚠ = Vial of Decay (Source: Dead Bodies)<br>
❀ = Shifting Rose (Source: Shapeshifters)<br>
☀ = Essence of Sight (Source: Fixing Lights)<br>
◯ = Fragment of Discussions (Source: Groups of 3 or more people)<br>

_Potions_<br>
Potion of Death => Kills the nearest player<br>
Castling Brew => Applies a 1-time use shield to the player<br>
Potion of Sight => Increases players vision for 60 seconds OR removes sabotage vision<br>
Warp Potion => Teleports you and a random player<br>
Mechanic's Mix => Allows player to instant fix next sabotage<br>
Leader Potion => Gives +1 vote during the next meeting<br>
Serene's Grace => Reveals the role of the most nearby player<br>
Unstable Concoction => Mutates into a random potion<br>

_Potion Ingredients_<br>
Potion of Death: ⚠ Vial of Decay + ◆ Base Catalyst Amount
Castling Brew: ◆ (2) Catalyst +  ◆ Base Catalyst Amount
Potion of Sight: ☀ Essence of Sight + ◆ Base Catalyst Amount
Warp Potion: Θ Theta Rift + ◆ Base Catalyst Amount
Mechanic's Mix: Fragment of Discussions + ◆ Base Catalyst Amount
Leader Potion: Fragment of Discussions + ◆ Base Catalyst Amount
Serene Grace: (2) Shifting Rose + ◆ Base Catalyst Amount
Unstable Concoction: (2) Theta Rift + ◆ Base Catalyst Amount

__Actions__: <br>
__Long Hold Pet Button__*: <br>
_Outside Crafting_: Brings you to the Crafting Menu<br>
_Inside Crafting_: Close the Crafting Menu (also creates a potion if selected and all ingredients are collected)<br>
_With Potion_: Use a crafted potion<br>

__Pet Button__**:<br>
_Outside Crafting_: Picks up any ingredients in the area<br>
_Inside Crafting_: Scrolls through potions<br>

*Notes* <br>
*Hold pet button long enough that you see the petting animation multiple times.<br>
**Hold pet button just long enough that you only see the petting animation one time.<br>

#### Role Description
Alchemist is a jack-of-all-trades crewmate role that collects "ingredients". Ingredients can be found in the following ways:<br>
  • Catalyst - Found by completing tasks<br>
  • Essence of Sight - Found when helping fix lights<br>
  • Fragment of Discussions - Found randomly in groups of 3 or more players<br>
  • Shifting Rose - Found after a player shapeshifts<br>
  • Theta Rift - Found randomly<br>
  • Vital of Decay - Found off dead bodies<br>

The Alchemist can use their pet button to pick up these ingredients, and will get a message below their name saying: "Found: [Ingredient Name]".<br>

The Alchemist uses ingredients to craft potions, to switch into "crafting mode" the Alchemist must hold down their pet button. Once in crafting mode, the pet button can be used to switch the next crafted potion.<br>

If in the crafting menu, the Alchemist can hold down their pet button to exit it. If the Alchemist has all of the necessary ingredients to craft the potion they were on, the potion will begin crafting as they hold the pet button.<br>

Once the Alchemist has a potion, they can hold down the pet button to use it, consuming it.<br>

## Game Options

|         Name         |                        Description                        |     Type     |  Default  | 
| -------------------- | --------------------------------------------------------- | :----------: | :-------: |
| Alchemist            | The probability of the Alchemist appearing                |  Percentage  |    0%     |
| Maximum              | How many Alchemists should spawn                          |    Number    |     1     |
| Base Catalyst Amount | The amount of catalysts needed for potions                |    Number    |     2     |
| Potion of Death      | Whether Potion of Death is a crafting option              |    Toggle    |    ON     |
| Castling Brew        | Whether Castling Brew is a crafting option                |    Toggle    |    ON     |
| Potion of Sight      | Whether Potion of Sight is a crafting option              |    Toggle    |    ON     |
| Warp Potion          | Whether Warp Potion is a crafting option                  |    Toggle    |    ON     |
| Mechanic's Mix       | Whether Mechanic's Mix is a crafting option               |    Toggle    |    ON     |
| Leader Potion        | Whether Leader Potion is a crafting option                |    Toggle    |    ON     |
| Serene Grace         | Whether Serene Grace is a crafting option                 |    Toggle    |    ON     |
| Unstable Concoction  | Whether Unstable Concoction is a crafting option          |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Bastion 

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Engineer<br>
__Ability__: Plant Bombs In Vents<br>
__Indicatior/Symbols__: Counter Showing Remaining Amount Of Vents They Can Trap<br>

`Originally Developed By: Discussions`<br>
`Idea By: Mek`<br>

#### Role Description
Use the Vent button to plant a bomb in a vent. This will kill the next player who uses that vent.<br>
Bombs last for one round only. Vents will be reset at each meeting.<br><br>
Be careful! The Bastion can bomb themself by using a vent they've already planted a bomb in.<br>

### Game Options (incomplete)
|        Name         |                       Description                       |     Type     |  Default  | 
| ------------------- | ------------------------------------------------------- | :----------: | :-------: |
| Bastion             | The probability of the Bastion appearing                |  Percentage  |    0%     |
| Maximum             | How many Bastions should spawn                          |    Number    |     1     |
| Plant Bomb Cooldown | The cooldown of the Bastion's Vent button               |     Time     |   19.5s   |
| Bombs Per Round     | How many bombs can be planted per round                 |    Number    |     ∞     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Bodyguard

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Sacrifice's Their Life To Protect Another<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea By: Det`<br>

#### Role Description
The first player voted becomes the Bodyguard’s Target. This will not count as a vote.<br>
Whenever the Bodyguard’s Target is attacked, the attacker is killed alongside the Bodyguard.<br>
The Bodyguard may skip freely before their target is locked in and vote freely after their target has been locked in.<br>

### Game Options
|                 Name                   |                                     Description                                 |     Type     |   Default   | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :---------: |
| Bodyguard                              | The probability of the Bodyguard appearing                                      |  Percentage  |     0%      |
| Maximum                                | How many Bodyguards should spawn                                                |    Number    |     1       |
| Change Guarded Player                  | Options for when to change the Guarded player                                   |    Toggle    | After Death | 
| Protect Against Beneficial Interations | Whether the Bodyguard protects against Beneficial Interactions (e.g. Crusader)  |    Toggle    |     OFF     |
| Protect Against Neutral Interactions   | Whether the Bodyguard protects agianst Neutral Interactions (e.g. Investigator) |    Toggle    |     ON      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Chameleon

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Engineer<br>
__Ability__: Camouflage With Your Environment<br>
__Indicatior/Symbols__: Invisible Duration Counter<br>

#### Role Description
The Chameleon can use their Vent button to temporarily turn invisible. Their invisible duration is displayed below their name, and after a fixed duration they will re-appear in their current spot.

### Game Options
|                 Name                   |                                     Description                                 |     Type     |  Default | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :------: |
| Chameleon                              | The probability of the Chameleon appearing                                      |  Percentage  |    0%    |
| Maximum                                | How many Chameleons should spawn                                                |    Number    |     1    |
| Invisibility Duration                  | The duration of the Chameleon's invisibility                                    |     Time     |    10s   |        
| Invisibility Cooldown                  | The cooldown of the Chameleon's invisibility ability                            |     Time     |    10s   |

_Vent button cooldown = Invisibility Duration + Invisibility Cooldown_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Charmer

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Charm Enemies To Join Your Team.<br>
__Indicatior/Symbols__: Charmed Players Receive Indicator That They've Been Charmed<br>

#### Role Description
When the Charmer uses their Pet/Kill button on an impostor or neutral killer, they become charmed and join the crewmates team. Charmed players will know they've been charmed, and lose the ability to kill crewmates.  If the Charmer charms a crewmate, they misfire and die.

### Game Options
|                 Name                   |                                     Description                                 |     Type     |   Default  | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :--------: |
| Charmer                                | The probability of the Charmer appearing                                        |  Percentage  |    0%      |
| Maximum                                | How many Charmer should spawn                                                   |    Number    |     1      |
| Ability Button                         | Choice between Pet/Kill for the Charmer's ability                               |    Toggle    | Pet Button |
| ┗ Tasks Needed For Ability             | How many tasks need to be completed to use Charm ability                        |    Number    |     0      |
| Charming Cooldown                      | The cooldown of the Charmer's Charm ability                                     |     Time     |    60s     |
| Charmed Players Win With Crew          | Whether charmed players win with Crewmates                                      |    Toggle    |    ON      |
| Break Charm On Charmer Death           | Whether charmed players remain on the Crewmates team upon the Charmer's Death   |    Toggle    |    ON      |
| Max Charmed Players                    | How many players the Charmer can charm onto the Crewmate team                   |    Number    |     ∞      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Crusader

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Impostor<br>
__Ability__: Protect Players From Attacks<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea By: Det`<br>

#### Role Description
The Crusader works like a living Guardian Angel from Vanilla Amoung Us.<br>
Use the Kill button to select a target.<br>
This target will be protected from attacks.<br>

### Game Options
|                 Name                    |                                     Description                                 |     Type     | Default | 
| --------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :-----: |
| Crusader                                | The probability of the Crusader appearing                                       |  Percentage  |   0%    |
| Maximum                                 | How many Crusaders should spawn                                                 |    Number    |    1    |
| Protect Against Beneficial Interactions | Whether the Crusader protects against Beneficial Interactions (e.g. Crusader)   |    Toggle    |   OFF   |
| Protect Against Neutral Interactions    | Whether the Crusader protects against Neutral Interactions (e.g. Investigator)  |    Toggle    |   ON    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Demolitionist

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Bombs their Killer<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea By: Mek`<br>

#### Role Description
When the Demolitionist is killed, they bomb the ground, giving the killer a few seconds to find a vent.<br>
If the killer does not vent in time, they are bombed.<br>
The killer is notified that they have killed the demolitionist by their name/role.<br>

### Game Options
|     Name      |                 Description                    |     Type     |  Default  | 
| ------------- | ---------------------------------------------- | :----------: | :-------: |
| Demolitionist | The probability of the Demolitionist appearing |  Percentage  |    0%     |
| Maximum       | How many Demolitionists should spawn           |    Number    |     1     |
| Demo Time     | Amount of time the killer has to find a vent   |      Time    |    1.5    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Dictator

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Pick Who To Vote Out<br>
__Indicatior/Symbols__: Counter (During Meetings) Showing Number Of Dictates Before Suicide<br>

`Originally Developed By: そうくん`<br>
`Idea By: そうくん`

#### Role Description
Three things happen when the Dictator votes for someone in meeting:<br>
1. They forcibly end the meeting.<br>
2. The player they voted for is exiled.<br>
3. Sacrifice themself in the name of justice (they die) if they have no more dictate votes left.<br>

### Game Options
|               Name               |                            Description                           |     Type     |  Default  | 
| -------------------------------- | ---------------------------------------------------------------- | :----------: | :-------: |
| Dictator                         | The probability of the Dictator appearing                        |  Percentage  |    0%     |
| Maximum                          | How many Dictators should spawn                                  |    Number    |     1     |
| Number of Dictates               | How many times Dictator can use their ability                    |    Number    |     1     |
| ┗ Show Dictate at End of Meeting | Shows Dictate message at end of meeting (rather than right away) |    Toggle    |    ON     |
| Suicide if Crewmate Executed     | Whether Dictator suicides when executing a Crewmate              |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Doctor

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Scientist<br>
__Ability__: Can See How Players Died<br>
__Indicatior/Symbols__: Cause Of Death Displayed In Meetings<br>

`Originally Developed By: Town of Host`<br>
`Idea By: Nebula on the Ship`<br>

#### Role Description
The Doctor has a portable vitals panel just like the vanilla role, Scientist. Check this regularly to get an approximated time of death.<br>
While in meeting (and by closing the chat), the Doctor can see a player’s cause of death in parentheses next to their name.<br>

### Game Options
|          Name           |                    Description                         |     Type     |  Default  | 
| ----------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Doctor                  | The probability of the Doctor appearing                |  Percentage  |    0%     |
| Maximum                 | How many Doctors should spawn                          |    Number    |     1     |
| Vitals Cooldown         | The Cooldown of the Doctor's Vitals button             |     Time     |    40s    |
| Vitals Battery Charge   | The amount of time the Doctor can View portable vitals |     Time     |   14.5s   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Escort 

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Impostor<br>
__Ability__: Role Block Players<br>
__Indicatior/Symbols__: "RB" Indicator On Roleblocked Player<br>

`Originally Developed By: Discussions`<br>
`Idea By: Loonie`<br>

#### Role Description
Use the Pet button to roleblock<br>
Role blocks prevent kills, reports, and venting.<br>
Cannot roleblock The Glitch.<br>

### Game Options
|            Name               |                      Description                       |     Type     |    Default    | 
| ----------------------------- | ------------------------------------------------------ | :----------: | :-----------: |
| Escort                        | The probability of the Escort appearing                |  Percentage  |      0%       |
| Maximum                       | How many Escorts should spawn                          |    Number    |       1       |
| Roleblock Cooldown            | The cooldown of the Escort's ability                   |     Time     |      45s      |
| Roleblock Duration            | The duration of the Escort's ability                   |     Time     | Until Meeting |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Ex-Convict

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Prepare A Location, Then Escape!<br>
__Indicatior/Symbols__: Text Cooldown Displaying Time Until Able to Escape & Until Next Mark<br>

#### Role Description
First use Pet button to mark a location, then after a set cooldown, you can re-use the Pet button to teleport back to your marked location. This will then put the mark ability back on cooldown.

### Game Options
|            Name               |                      Description                       |     Type     | Default | 
| ----------------------------- | ------------------------------------------------------ | :----------: | :-----: |
| Ex-Convict                    | The probability of the Ex-Convict appearing            |  Percentage  |    0%   |
| Maximum                       | How many Ex-Convicts should spawn                      |    Number    |    1    |
| Cooldown After Mark           | The cooldown of the Ex-Convict's mark ability          |     Time     |    5s   |
| Cooldown After Escape         | The cooldown of the Ex-Convict's escape ability        |     Time     |   40s   |
| Clear Mark After Meeting      | Whether Ex-Convict's mark stays after meeting          |    Toggle    |    ON   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Herbalist

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Plant Blooms to Slowly Gather Info<br>
__Indicatior/Symbols__: Bloom Counter On Seeded Players & Plant Bloom Cooldown Counter<br>

#### Role Description
Use your Pet button to plant a seed on a player. After a set period of time, that player's "bloom counter" will increase. After a set number of blooms, use your pet button to reveal that player's role. After a player's role has been revealed, you can continue to reveal it to the nearest player by using the pet button on the same player.

### Game Options
|                 Name                   |                                     Description                                           |     Type     |  Default  | 
| -------------------------------------- | ----------------------------------------------------------------------------------------- | :----------: | :-------: |
| Herbalist                              | The probability of the Herbalist appearing                                                |  Percentage  |     0%    |
| Maximum                                | How many Herbalists should spawn                                                          |    Number    |     1     |
| Time Until Bloom                       | The amount of time it takes for the seed to bloom                                         |     Time     |    15s    |
| Blooms Until Role Reveal               | How many blooms are needed before role reveal                                             |    Number    |     3     |
| Plant Bloom Cooldown                   | The cooldown of the Herbalist's seed planting ability                                     |     Time     |    20s    |
| Reveal on Bloom                        | Whether the Herbalist needs to use the pet button to reveal the role on the seeded player |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Investigator

<img align="right" width="" height="300" src="">

__Faction__: Crewmates<br>
__Base__: Impostor/Crewmate<br>
__Ability__: Investigate Roles<br>
__Indicatior/Symbols__: Player's Name Changes Based On "Good" or "Bad"<br>

`Originally Developed By: Discussions`<br>
`Idea By: Town of Us Reactivated`<br>

#### Role Description
Use the Kill button to investigate if the player is good or bad. In general, red is bad & green is good.<br>
Be wary of how 'bad' the player with the red name is. The Sheriff or Veteran can end up with a red name in some lobbies!<br>

__*Red = Bad*__ <br>
 - __Impostors__ (always)<br>
 - __Neutral Killing__ (predetermined by host)<br>
 - __Neutral Passive__ (predetermined by host)<br>
 - __Crewmate Killing__ (predetermined by host)<br>
 - __Madmate__ (predetermined by host)<br><br>
 
 
__*Green = Good*__ <br>
 - __Crewmates__ (always)<br>
 - __Neutral Killing__ (predetermined by host)<br>
 - __Neutral Passive__ (predetermined by host)<br>
 - __Crewmate Killing__ (predetermined by host)<br>
 - __Madmate__ (predetermined by host)<br><br>

### Game Options
|          Name            |                          Description                             |    Type    |  Default  | 
| ------------------------ | ---------------------------------------------------------------- | :--------: | :-------: |
| Investigator             | The probability of the Investigator appearing                    | Percentage |     0%    |
| Maximum                  | How many Investigators should spawn                              |   Number   |     1     |
| Investigate Cooldown     | The cooldown of the Investigator's Kill button                   |    Time    |   27.5s   |
| Neutral Killing are Red  | Whether Neutral Killing roles appear red when investigated       |   Toggle   |    OFF    | 
| ┣ AgiTater               | Whether AgiTater will show a red name when investiagted          |   Toggle   |  Enabled  |
| ┣ Arsonist               | Whether Arsonist will show a red name when investigated          |   Toggle   |  Enabled  |
| ┣ Blood Knight           | Whether Blood Knight will show a red name when investigated      |   Toggle   |  Enabled  |
| ┣ Demon                  | Whether Demon will show a red name when investigated             |   Toggle   |  Enabled  |
| ┣ Egoist                 | Whether Egoist will show a red name when investigated            |   Toggle   |  Enabled  |
| ┣ The Glitch             | Whether The Glitch will show a red name when investigated        |   Toggle   |  Enabled  |
| ┣ Hitman                 | Whether Hitman will show a red name when investigated            |   Toggle   |  Enabled  |
| ┣ Jackal                 | Whether Jackal will show a red name when investigated            |   Toggle   |  Enabled  |
| ┣ Juggernaut             | Whether Juggernaut will show a red name when investigated        |   Toggle   |  Enabled  |
| ┣ Marksman               | Whether Marksman will show a red name when investigated          |   Toggle   |  Enabled  |
| ┣ Occultist              | Whether Occultist will show a red name when investigated         |   Toggle   |  Enabled  |
| ┣ Pelican                | Whether Pelican will show a red name when investigated           |   Toggle   |  Enabled  |
| ┣ Pestilence             | Whether Pestilence will show a red name when investigated        |   Toggle   |  Enabled  |
| ┣ Plague Bearer          | Whether Plague Bearer will show a red name when investigated     |   Toggle   |  Enabled  |
| ┣ Retributionist         | Whether Retributionish will show a red name when investigated    |   Toggle   |  Enabled  |
| ┣ Ruthless Romantic      | Whether Ruthless Romantic will show a red name when investigated |   Toggle   |  Enabled  |
| ┗ Werewolf               | Whether Werewolf will show a red name when investigated          |   Toggle   |  Enabled  | 
| Neutral Passive are Red  | Whether Neutral Passive roles appear red when investigated       |   Toggle   |    OFF    |
| ┣ Amalgamation           | Whether Amalgamation will show a red name when investigated      |   Toggle   |  Enabled  |
| ┣ Amnesiac               | Whether Amnesiac will show a red name when investigated          |   Toggle   |  Enabled  |
| ┣ Archangel              | Whether Archangel will show a red name when investigated         |   Toggle   |  Enabled  |
| ┣ Copycat                | Whether Copycat will show a red name when investigated           |   Toggle   |  Enabled  | 
| ┣ Executioner            | Whether Executioner will show a red name when investigated       |   Toggle   |  Enabled  |
| ┣ Hacker                 | Whether Hacker will show a red name when investigated            |   Toggle   |  Enabled  |
| ┣ Jester                 | Whether Jester will show a red name when investigated            |   Toggle   |  Enabled  |
| ┣ Opportunist            | Whether Opporttunist will show a red name when investigated      |   Toggle   |  Enabled  | 
| ┣ Phantom                | Whether Phantom will show a red name when investigated           |   Toggle   |  Enabled  |
| ┣ Postman                | Whether Postman will show a red name when investigated           |   Toggle   |  Enabled  |
| ┣ Schrodinger's Cat      | Whether Schrodinger's Cat will show a red name when investigated |   Toggle   |  Enabled  |
| ┣ Survivor               | Whether Survivor will show a red name when investigated          |   Toggle   |  Enabled  |
| ┣ Terrorist              | Whether Terrorist will show a red name when investigated         |   Toggle   |  Enabled  | 
| ┗ Vulture                | Whether Vulture will show a red name when investigated           |   Toggle   |  Enabled  |
| Madmates are Red         | Whether Madmate roles appear red when investigated               |   Toggle   |    OFF    |
| ┣ CrewPostor             | Whether CrewPostor will show a red name when investigated        |   Toggle   |  Enabled  |
| ┣ Mad Guardian           | Whether Mad Guardian will show a red name when investigated      |   Toggle   |  Enabled  |
| ┣ Madmate                | Whether Madmate will show a red name when investigated           |   Toggle   |  Enabled  |
| ┣ Mad Snitch             | Whether Mad Snitch will show a red name when investigated        |   Toggle   |  Enabled  |
| ┗ Parasite               | Whether Parasite will show a red name when investigated          |   Toggle   |  Enabled  |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mayor

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate or Engineer<br>
__Ability__: Additional Votes / Venting Calls Meetings<br>
__Indicatior/Symbols__: Counter Showing Number of Pocket Meetings<br>

`Originally Developed By: Discussions`<br>
`Idea By: The Other Roles`<br>

#### Role Description
Mayor’s vote is counted multiple times (predetermined by the host in settings).<br>
Depending on the options, they can call emergency meetings by using the Pet button.<br>
Additionally, there's an option where Mayor has to reveal before gaining additional votes (reveal by voting yourself)<br>

### Game Options
|         Name           |                       Description                       |     Type     |  Default  | 
| ---------------------- | ------------------------------------------------------- | :----------: | :-------: |
| Mayor                  | The probability of the Mayor appearing                  |  Percentage  |    0%     |
| Maximum                | How many Mayors should spawn                            |    Number    |     1     |
| Reveal for Votes       | Reveal extra votes from Mayor                           |    Toggle    |    OFF    |
| Mayor Additional Votes | How many additional votes the Mayor has                 |    Number    |     1     |
| Pocket Meeting         | Whether the Mayor has pocket meetings                   |    Toggle    |     ON    |
| ┗ Number Of Uses       | How many pocket meetings the Mayor has                  |    Number    |     3     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mechanic

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Engineer<br>
__Ability__: Use Vents<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Innersloth`<br>

#### Role Description
The Mechanic can use vents to travel around the map.<br>
They are restricted by the Vent Use Cooldown & Max Time In Vents Options used for vanilla Engineer.<br>
The Mechanic is a renamed Engineer from vanilla Among Us.<br>

### Game Options
|           Name             |                           Description                       |     Type     |  Default  | 
| -------------------------- | ----------------------------------------------------------- | :----------: | :-------: |
| Mechanic                   | The probability of the Mechanic appearing                   |  Percentage  |    0%     |
| Maximum                    | How many Mechanics should spawn                             |    Number    |     1     |
| Vent Cooldown              | The cooldown of the Mechanic's Vent button                  |     Time     |    40s    |
| Vent Duration              | The amount of time the Mechanic can stay in a vent          |     Time     |   14.5s   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Medic

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Shield a Player From Attacks<br>
__Indicatior/Symbols__: Small "+" Mark Showing Shielded Player<br>

`Originally Developed By: Discussions`<br>
`Idea By: Town of Us Reactivated`<br>

#### Role Description
The Medic is able to vote a player to shield. Based on host's options, the Medic may be able to change their protected player during following meetings.

### Game Options 
|             Name               |                           Description                       |     Type     |   Default   | 
| ------------------------------ | ----------------------------------------------------------- | :----------: | :---------: |
| Medic                          | The probability of the Medic appearing                      |  Percentage  |     0%      |
| Maximum                        | How many Medics should spawn                                |    Number    |      1      |
| Change Guarded Player          | Options for if/when to change guarded player                |    Toggle    | After Death |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Medium

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Reveal The Killers Role When Reporting<br>
__Indicatior/Symbols__: Medium <br>

`Originally Developed By: Discussions`<br>
`Idea By: Town of Us Reactivated`<br>

#### Role Description
Use the Report button to report a body.<br>
In meeting chat, the Medium will receive a message revealing the role of the reported player's killer.<br>
Medium can only see killer's role if they reported the body themselves.<br>
Depending on host's settings, they may also see an arrow pointing to bodies.<br>

### Game Options 
|             Name               |                           Description                       |     Type     |  Default  | 
| ------------------------------ | ----------------------------------------------------------- | :----------: | :-------: |
| Medium                         | The probability of the Medium appearing                     |  Percentage  |    0%     |
| Maximum                        | How many Mediums should spawn                               |    Number    |     1     |
| Has Arrows to Bodies           | Whether the Medium will see an arrow point to bodies        |    Toggle    |    OFF    | 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Mystic

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Notified When Players Are Killed<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea By: Town of Us Reactivated`<br>

#### Role Description
When a player is killed, Mystic receives a single flash and alert. It is very similar to when the reactor is sabotaged. Use this alert to estimate time of death.

### Game Options
|         Name         |                      Description                       |     Type     |  Default  | 
| -------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Mystic               | The probability of the Mystic appearing                |  Percentage  |    0%     |
| Maximum              | How many Mystics should spawn                          |    Number    |     1     |
| Mystic is a Modifier | Whether Mystic is a Modifier instead of a role         |    Toggle    |    OFF    |
| Flash Duration       | Amount of time a Flash alert is present                |     Time     |    0.5s   |
| Send Audio Alert     | Whether there is an audio alert                        |    ON/OFF    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Observer

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Increased Vision<br>
__Indicatior/Symbols__: None<br>

#### Role Description
Finish tasks to gain vision. Depending on the host's options, you may gain a small vision boost upon completing each task, or, a large vision boost when all tasks have been complete.<br>
Additionally, if enabled, you'll be able to see even during sabotages.<br>

### Game Options
|               Name                       |                              Description                                            |     Type     |  Default  | 
| ---------------------------------------- | ----------------------------------------------------------------------------------- | :----------: | :-------: |
| Observer                                 | The probability of the Observer appearing                                           |  Percentage  |    0%     |
| Maximum                                  | How many Obervers should spawn                                                      |    Number    |     1     |
| Slowly Gains Vision                      | Whether the Observer gains vision with each task completed or total task completion |    Toggle    |    OFF    |
| ┗ Vision Gain On Task Complete           | The amount of vision increase the Observer receives for each task they complete     |   Multiplier |   0.15x   |
| Override Starting Vision                 | Whether Observer starts with a different vision other than default                  |    Toggle    |    OFF    |
| ┗ Starting Vision Modifier               | How much vision the Observer has before any tasks are completed                     |   Multiplier |   0.25x   |
| Finished Tasked Vision                   | The final vision distance Observer has when all tasks are completed                 |   Multiplier |   2.25x   |
| Lights Immunity If Tasks Finished        | Whether Observer is unaffected by Lights Sabotage or not                            |    Toggle    |    ON     |
 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Oracle

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Reveal A Role Upon Death<br>
__Indicatior/Symbols__: After the Oracle dies, the targeted player will have their role shown to everyone with a bluish-purple gradient<br>

`Originally Developed By: Discussions`<br>
`Idea By: Det`<br>

#### Role Description
The first player voted by the Oracle becomes the Oracle’s Target. This will not count as a vote.<br>
When the Oracle dies, the Target’s role is revealed to everyone.<br>
The Oracle may skip freely before their target is locked in and vote freely after their target has been locked in.<br>
The Oracle can choose to reveal their own role if they wish by voting themselves.<br>

### Game Options
|   Name  |                     Description                        |     Type     |  Default  | 
| ------- | ------------------------------------------------------ | :----------: | :-------: |
| Oracle  | The probability of the Oracle appearing                |  Percentage  |    0%     |
| Maximum | How many Oracles should spawn                          |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Physicist

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Scientist<br>
__Ability__: Can See Vitals<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Innersloth`<br>

#### Role Description
The Physicists have a portable vitals monitor that can be accessed anywhere on the map.<br>
The Physicist is a renamed Scientist from vanilla Amoung Us.<br>

### Game Options
|          Name           |                        Description                        |     Type     |  Default  | 
| ----------------------- | --------------------------------------------------------- | :----------: | :-------: |
| Physicist               | The probability of the Physicist appearing                |  Percentage  |    0%     |
| Maximum                 | How many Physicists should spawn                          |    Number    |     1     |
| Vitals Cooldown         | The Cooldown of the Physicist's Vitals button             |     Time     |    40s    |
| Vitals Battery Charge   | The amount of time the Physicist can View portable vitals |     Time     |   14.5s   |


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Psychic 

<img align="right" width="" height="300" src="">

__Faction__: Crewmates<br>
__Base__: Crewmate<br>
__Ability__: See A Potential Evil Player<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea By: Loonie`

#### Role Description
The Psychic has the ability to see potential evils during a meeting.<br>
Three players will be highlighted in red, at least one of them is evil. The number of players highlighted can be adjusted by the host.<br>

### Game Options (incomplete)
|              Name             |                      Description                                  |    Type    |  Default  | 
| ----------------------------- | ----------------------------------------------------------------- | :--------: | :-------: |
| Psychic                       | The probability of the Psychic appearing                          | Percentage |    0%     |
| Maximum                       | How many Psychics should spawn                                    |   Number   |     1     |
| Highlighted Players           | How many players are highlighted during meeting                   |   Number   |     3     |
| All Killing Roles are Evil    | Whether all killing roles are considered evil (including sheriff) |   Toggle   |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Repairman

<img align="right" width="" height="300" src="">

__Faction__: Crewmates<br>
__Base__: Crewmate/Engineer<br>
__Ability__: Clear Sabotages Without Help<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: 空き瓶/EmptyBottle`<br> 
`Idea By: 空き瓶/EmptyBottle (SabotageMaster)`

#### Role Description
Repairman can fast-fix sabotages that typically require two players (e.g. reactor) on their own.<br>
Lights can be fixed by touching a single lever.<br>
Opening a door in Polus or The Airship will open all the linked doors.<br>

### Game Options
|            Name           |                   Description                 |     Type     |  Default  | 
| ------------------------- | --------------------------------------------- | :----------: | :-------: |
| Sabotage Master           | The probability of the Repairman appearing    |  Percentage  |    0%     |
| Maximum                   | How many Repairmans should spawn              |    Number    |     1     |
| Repairman Can Vent        | Whether the Repairman can vent                |    Toggle    |    ON     | 
| ┣ Vent Cooldown           | The cooldown of the Repairman's vent button   |     Time     |    40s    | 
| ┗ Vent Duration           | How long the Repairman can stay inside a vent |     Time     |    15s    | 
| Fast Fixes Lights         | Whether Repairman can fast-fix Lights         |    Toggle    |    ON     |
| Fast Fixes Reactor        | Whether Repairman can fast-fix Reactor        |    Toggle    |    ON     |
| Fast Fixes Oxygen         | Whether Repairman can fast-fix Oxygen         |    Toggle    |    ON     |
| Fast Fixes Communications | Whether Repairman can fast-fix Communications |    Toggle    |    ON     |
| Fast Fixes Doors          | Whether Repairman can fast-fix Doors          |    Toggle    |    ON     |
| Fast Fixes Crash Course   | Whether Repairman can fast-fix Crash Course   |    Toggle    |    ON     |


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Sheriff

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Impostor/Crewmate<br>
__Ability__: Can Shoot Impostors<br>
__Indicatior/Symbols__: Counter showing number of bullets<br>

`Originally Developed By: Town of Host` <br>
`Idea From: Woodi-dev`

#### Role Description
The Sheriff can kill Impostors.<br>
Be Careful! The Sheriff will misfire (kill themself) if they shoot a crewmate or a neutral not allowed by host.<br>
Additionally (depending on settings) they may have no tasks.<br>

### Game Options
|           Name           |                           Description                        |         Type        |  Default  | 
| ------------------------ | ------------------------------------------------------------ | :-----------------: | :-------: |
| Sheriff                  | The probability of the Sheriff appearing                     |      Percentage     |    0%     |
| Maximum                  | How many Sheriffs should spawn                               |        Number       |     1     |
| Kill Target On Misfire   | Whether Sheriff will kill their target when misfiring        |        Toggle       |    OFF    |
| Kill Cooldown            | The Cooldown for the Sheriff's Kill/Pet button               |         Time        |    25s    |
| Total Shots              | The total amount of shots (kills) the Sheriff can make       |        Number       |     5     |
| One Shot Per Round       | Whether the Sheriff can make multiple shots per round or not |        Toggle       |    ON     |
| Sheriff Action Button    | Toggles the Kill/Pet Button for the Sheriff's ability        |        Toggle       |   Kill    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Snitch 

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Finish Tasks To See Killers<br>
__Indicatior/Symbols__: ⚠ indicator when on task threshold<br>

`Originally Developed By: Town of Host`<br>
`Idea From: The Other Roles`<br>

#### Role Description
The Snitch can see Impostors (has option to see any neutral killers as well) once tasks are complete.<br>
When the Snitch has a certain number of tasks left (predetermined based on host's settings), they will be revealed to the killers with a ⚠ indicator.<br>
Depending on the settings, when their tasks are completed, the Snitch may also see arrows pointed in the direction of each player they're tracking.<br>

### Game Options
|               Name               |                              Description                              |     Type     |  Default  | 
| -------------------------------- | --------------------------------------------------------------------- | :----------: | :-------: |
| Snitch                           | The probability of the Snitch appearing                               |  Percentage  |    0%     |
| Maximum                          | How many Snitches should spawn                                        |    Number    |     1     |
| Remaining Task Warning           | How many tasks the Snitch will have remaining to alert the killers    |    Number    |     2     |
| Evil Have Arrow to Snitch        | Whether evil players will have an arrow to the Snitch                 |    Toggle    |    ON     |
| Enable Arrow for Snitch          | Whether the Snitch will have arrows to the killers                    |    Toggle    |    ON     |
| ┗ Colored Arrow                  | Whether the arrows are colored based on role color                    |    Toggle    |    ON     |
| Snitch can Track Any Killing     | Whether Snitch can track any killers                                  |    Toggle    |    ON     |
| Override Snitch's Tasks          | Options to customize Snitch's tasks                                   |    Toggle    |   OFF     |
| ┣ Allow Common Tasks             | Whether the Snitch will receive Common Tasks                          |    Toggle    |    ON     |
| ┣ Snitch Long Tasks              | How many Long Tasks will be assigned to the Snitch                    |    Number    |     5     |
| ┗ Snitch Short Tasks             | How many Short Tasks will be assigned to the Snitch                   |    Number    |     6     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Speedrunner 

<img align="right" width="" height="300" src="">

__Faction__: Crewmates<br>
__Base__: Crewmate<br>
__Ability__: Increased Speed Upon Task Completion<br>
__Indicatior/Symbols__: None<br>

#### Role Description
Finish tasks to gain a speed boost! Depending on the host's options, you may gain a small speed boost (possibly temporarily depending on settings) after completing singular tasks, or, get a large speed boost after reaching a task-threshold.

### Game Options
|                 Name                   |                                         Description                                     |     Type     |  Default  | 
| -------------------------------------- | --------------------------------------------------------------------------------------- | :----------: | :-------: |
| Speedrunner                            | The probability of the Speedrunner appearing                                            |  Percentage  |    0%     |
| Maximum                                | How many Speedrunners should spawn                                                      |    Number    |     1     |
| Temporary Boost Upon Finishing Task    | Whether the Speedrunner will receive a temporary small boost after finishing each task  |  Multiplier  |   0.1x    |    
| ┗ Temporary Boost Duration             | How long the temporary speed boost lasts after each completed task                      |     Time     |    3s     | 
| Permanent Speed Gain per Task          | How much of a permanent boost the Speedrunner gets after completing each task           |  Multiplier  |    0.1x   | 
| Tasks Remaining Until Main Speed Boost | How many tasks need to be completed to receive Final Speed Boost                        |    Number    |     2     |                       
| ┗ Final Speed Boost                    | Final Player Speed when Speedrunner completes Tasks Until Speed Boost                   |  Multiplier  |   2.25x   |                    

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Swapper 

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Swap Votes During Meeting<br>
__Indicatior/Symbols__: None<br>

`Idea From: Town of Us Reactivated`

#### Role Description
The first two players you vote each meeting will have their votes swapped. After voting those players, you may vote as normal. Alternatively, you can skip at the start and continue to normal voting.

### Game Options
|      Name      |                       Description                       |     Type     |  Default  | 
| -------------- | ------------------------------------------------------- | :----------: | :-------: |
| Swapper        | The probability of the Swapper appearing                |  Percentage  |    0%     |
| Maximum        | How many Swappers should spawn                          |    Number    |     1     |
| Swaps Per Game | How many votes the Swapper can swap per game            |    Number    |     ∞     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Tracker 

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Track a player's movements<br>
__Indicatior/Symbols__: Arrow Pointing Towards Tracked Player<br>

`Idea From: Town of Us Reactivated`

#### Role Description
Once per meeting, select a player to track. You will have an arrow pointing towards that player until they die. If enabled, you may also use your pet button to temporarily track all dead bodies.

### Game Options
|               Name              |                       Description                       |     Type     |  Default  | 
| ------------------------------- | ------------------------------------------------------- | :----------: | :-------: |
| Tracker                         | The probability of the Tracker appearing                |  Percentage  |    0%     |
| Maximum                         | How many Trackers should spawn                          |    Number    |     1     |
| Arrow Update Rate               | The rate at which your tracking arrown updates          |     Time     |    1s     |
| Can Track Bodies                | If the Pet button ca nbe used to track bodies           |    Toggle    |    OFF    | 
| ┣ Can Track Unreportable Bodies | If, when tracking bodies, unreportable bodies are shown |    Toggle    |    ON     | 
| ┣ Track Body Duration           | The duration of the body tracking ability               |     Time     |   12.5s   |
| ┗ Track Body Cooldown           | The cooldown of the body tracking ability               |     Time     |    40s    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Transporter

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Transport Two Players<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea From: Town of Us Reactivated`<br>

#### Role Description
Use the Pet button and cause two random players to switch places.<br>
Make sure you have enough for the pet animation.<br>

### Game Options
|        Name          |                           Description                       |     Type     |  Default  | 
| -------------------- | ----------------------------------------------------------- | :----------: | :-------: |
| Transporter          | The probability of the Transporter appearing                |  Percentage  |    0%     |
| Maximum              | How many Transporters should spawn                          |    Number    |     1     |
| Number of Transports | How many times the Transporter may use it's ability         |    Number    |    25     |
| Transport Cooldown   | The cooldown of the Transport ability                       |     Time     |    30     |      

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Trapster 

<img align="right" width="" height="300" src="">

__Faction__: Crewmates<br>
__Base__: Crewmate<br>
__Ability__: Trap Their Killers<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: そうくん`<br>
`Idea By: 宿主ランニング`<br>

#### Role Description
Upon death, Trapster freezes their killer in place for a few seconds.<br>

### Game Options
|           Name          |                        Description                     |     Type     |  Default  | 
| ----------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Trapster                | The probability of the Trapster appearing              |  Percentage  |    0%     |
| Maximum                 | How many Trapsters should spawn                        |    Number    |     1     |
| Traps on Indirect Kills | Whether the Trapster's ability works on indirect kills |    Toggle    |    ON     |
| Trapped Duration        | The amount of time the killer is trapped for           |     Time     |    5s     |  

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Veteran

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Counterattacks Players' Kill Button<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: Discussions`<br>
`Idea From: Town of Us Reactivated`<br>

#### Role Description
When the Veteran is attacked while on Alert, the attack will backfire resulting in the attacker's death. Use the Pet button to activate the Veteran's ability.<br>
Pro Tip - Make sure you have enough room for the Pet animation!<br>      

### Game Options
|         Name           |                             Description                             |     Type     |  Default  | 
| ---------------------- | ------------------------------------------------------------------- | :----------: | :-------: |
| Veteran                | The probability of the Veteran appearing                            |  Percentage  |    0%     |
| Maximum                | How many Veterans should spawn                                      |    Number    |     1     |
| Number of Alerts       | How many times the Veteran can Alert (protect themself from attack) |    Number    |    10     |
| Alert Cooldown         | The Cooldown between Pet Button Usage (Alerts)                      |     Time     |    15s    |
| Alert Duration         | The amount of time the Veteran is Alerted for                       |     Time     |    3.5s   |
| Kill Crewmates         | Whether the Veteran can kill Crewmates or not                       |    Toggle    |    ON     |
| Kill While Transported | Wether the Veteran can kill the player they're transported with     |    Toggle    |    ON     |
| Kill Ranged Attackers  | Whether the Veteran can kill Ranged Attackers (e.g. Crewpostor)     |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Vigilante 

<img align="right" width="" height="300" src="">

__Faction__: Crewmate<br>
__Base__: Crewmate<br>
__Ability__: Guess Evil Roles To Eliminate Them<br>
__Indicatior/Symbols__: None<br>

`Originally Developed By: たんぽぽ`<br>
`Idea From: Town of Us Reactivated`<br>

#### Role Description
Vigilante is a nice guesser and part of the crewmate team.<br>
While in meeting the Vigilante's first vote locks in the player they're going to guess.<br>
The Vigilante's second guess locks in the role they're guessing.<Br>

### Game Options
|         Name           |                             Description                             |     Type     |  Default  | 
| ---------------------- | ------------------------------------------------------------------- | :----------: | :-------: |
| Vigilante              | The probability of the Vigilante appearing                          |  Percentage  |    0%     |
| Maximum                | How many Vigilantes should spawn                                    |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Neutral Killing

## AgiTater 

<img align="right" width="" height="300" src="">

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Pass The Bomb (Hot Potato)<br>
__Win Condition__: Be The Last Man Standing<br>

`Originally Developed by: Discussions`<br>
`Idea by Aaron Stuart`<br>

#### Role Description
As an AgiTater your goal is to give your bomb to another player using your kill button.<br>
Once another player is in range, the bomb will automatically be passed to them.<br>
This continues until a meeting is called (or optionally after a duration) where the last person holding the bomb is then eliminated.<br>

### Game Options (incomplete)
|            Name              |                                    Description                                 |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------------ | :----------: | :-------: |
| AgiTater                     | The probability of the AgiTater appearing                                      |  Percentage  |    0%     |
| Maximum                      | How many AgiTaters should spawn                                                |    Number    |     1     |
| Place Bomb Cooldown          | The cooldown of the AgiTater's ability to place bombs                          |    Number    |   Global  | 
| Explode On Meetings          | Whether bombed players explode when a meeting is called                        |    Toggle    |    ON     |
| Explode After Duration       | Whether bombed players will explode after a specific amount of time has passed |    Toggle    |    OFF    |
| Explode When Bombed Twice    | Whether bombed players will explode if they get a bomb for the second time     |    Toggle    |    OFF    |
| Bombs per Round              | How many bombs can be placed per round                                         |    Number    |     3     |
| Bomb Transfer Rate           | The time someone needs to be next to a player for the bomb to transfer         |     Time     |     1s    |

_The Global option for Place Bomb Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Arsonist

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Can Douse & Ignite Players<br>
__Win Condition__: Douse & Ignite All Living Players<br>

`Originally Developed by Discussions`
`Idea by TOR`

#### Role Description
Use the Kill button repeatedly next to a player to douse oil onto them. The player is doused when they are marked by a full orange circle.<br>
To win, douse all players and ignite them by using the Pet button.<br>

### Game Options
|            Name              |                                        Description                                      |     Type     |  Default  | 
| ---------------------------- | --------------------------------------------------------------------------------------- | :----------: | :-------: |
| Asronist                     | The probability of the Arsonist appearing                                               |  Percentage  |    0%     |
| Maximum                      | How many Arsonist should spawn                                                          |    Number    |     1     |
| Attacks to Complete Douse    | How many times the Arsonist needs to tap their Kill button to completely douse a player |    Number    |    19     |
| Can Ignite Anytime           | Whether the Arsonist can ignite players at any time throughout the game                 |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Blood Knight

__Faction__: Neutral Killing<br>
__Base__: Blood Knight<br>
__Ability__: Shielded With Each Kill<br>
__Win Condition__: Solo (be the last killer alive) <br>

`Originally Developed by Discussions`
`Idea by Mek`

#### Role Description
Each kill the Bloodknight does will protect them from attacks for a few seconds.<br>

### Game Options
|            Name              |                            Description                           |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------------- | :----------: | :-------: |
| Blood Knight                 | The probability of the Blood Knight appearing                    |  Percentage  |    0%     |
| Maximum                      | How many Blood Knights should spawn                              |    Number    |     1     |
| Kill Cooldown                | The cooldown of the Blood Knight's Kill button                   |     Time     |   Global  |
| Protection Duration          | The amount of time the Blood Knight is protected after they kill |     Time     |    15s    |
| Can Vent                     | Whether the Blood Knight can vent or not                         |    ON/OFF    |    ON     |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Demon

<img align="right" width="" height="300" src="">

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Attack Players To Reduce Their Health<br>
__Win Condition__: Solo (be the last player alive)<br>

#### Role Description
Demon is a neutral killing role whose goal is to kill all other players. When Demon is in the game all players spawn in with a green health bar over their heads. When the Demon attacks a player, their health bar will drop some health points. After fully reducing a player's health bar, that player will die. When Demon gets attacked, their health bar also decreases. The Demon heals some health when they kill players.

### Game Options
|                 Name                   |                                     Description                                 |     Type     |  Default  | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :-------: |
| Demon                                  | The probability of the Demon appearing                                          |  Percentage  |    0%     |
| Maximum                                | How many Demons should spawn                                                    |    Number    |     1     |
| Attack Cooldown                        | The cooldown of the Demon's Kill button                                         |     Time     |    2s     |    
| Damage Per Attack                      | The amount of damage given per attack (x/100)                                   |    Number    |    15     |
| Healing On Kill                        | The amount of health regained upon a victim's death (x/100)                     |    Number    |    20     |
| Damage Taken Per Attack                | The amount of damage the Demon receives when attacked (x/100)                   |    Number    |    35     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Egoist

__Faction__: Neutral Killing<br>
__Base__: Shapeshifter<br>
__Ability__: Can See Impostors<br>
__Win Condition__: Must Be Final Impostor<br>

`Originally Developed by そうくん`<br>
`Original Idea by しゅー`<br>

#### Role Description
Kill as a normal Impostor on the Impostor team . . . but Egoist is a traitor to the Impostors.<br>
Use Impostor-Seeing attribute to get them voted out (end game) and achieve a solo win.<br>
Impostors and Egoist cannot kill each other.<br>

### Game Options
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Egoist                       | The probability of the Egoist appearing                    |  Percentage  |    0%     |
| Maximum                      | How many Egoists should spawn                              |    Number    |     1     |
| Egoist is Shapeshifter       | Whether the base of Egoist is Shapeshifter                 |    Toggle    |    ON     |
| ┣ Shapeshift Cooldown        | The cooldown of the Egoist's Shapeshift button             |     Time     |    30s    |
| ┗ Shapeshift Duration        | The duration the Egoist can be shifted for                 |     Time     |    15s    |  

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Hitman

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Kill Players & Win With Anyone <br>
__Win Condition__: Stay Alive Until The End To Win<br>

`Originally Developed by Discussions`<br>
`Idea by Loonie`<br>

#### Role Description
Stay Alive! Hitman can win with most teams so long as they are alive at the end of the game.<br>
Use Kill button on anyone without consequence.<br>
Host can choose whether Hitman wins with Executioner/Jester.<br>

### Game Options (incomplete)
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Hitman                       | The probability of the Hitman appearing                    |  Percentage  |    0%     |
| Maximum                      | How many Hitmans should spawn                              |    Number    |     1     |
| Wins with Absolute Winners   | Whether Hitman wins with Absolute Winners (e.g. Jester)    |    Toggle    |   None    |
| ┣ Executioner                | Whether Hitman wins with Executioner                       |    Toggle    |    ON     |
| ┗ Jester                     | Whether Hitman wins with Jester                            |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Jackal

__Faction__: Neutral Killer<br>
__Base__: Impostor<br>
__Ability__: Can Kill Any Player Without Consequence<br>
__Win Condition__: Eliminate All Players to Win<br>

`Originally Developed by 空き瓶/EmptyBottle`<br>

#### Role Description
Kill everyone, including impostors, and be the last player standing.

### Game Options
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Jackal                       | The probability of the Jackal appearing                    |  Percentage  |    0%     |
| Maximum                      | How many Jackals should spawn                              |    Number    |     1     |
| Kill Cooldown                | The cooldown of the Jackal's Kill button                   |    Number    |  Global   |
| Can Vent                     | Whether the Jackal can vent                                |    Toggle    |    ON     |
| Can Sabotage                 | Whether the Jackal can sabotage                            |    Toggle    |    ON     |
| Impostor Vision              | Whether the Jackal has Impostor vision                     |    Toggle    |    ON     |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Juggernaut

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Decreased Kill Cooldown With Each Kill<br>
__Win Condition__: Kill Everyone & Be Last Player Alive<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
The Juggernaut starts with a higher kill cooldown, but with every kill, their cooldown decreases. They must kill everyone, including impostors, and be the last person standing.

### Game Options
|            Name              |                                 Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------ | :----------: | :-------: |
| Juggernaut                   | The probability of the Juggernaut appearing                              |  Percentage  |    0%     |
| Maximum                      | How many Juggernauts should spawn                                        |    Number    |     1     |
| Kill Cooldown                | The cooldown of the Juggernaut's Kill button                             |    Number    |   Global  |     
| Cooldown Reduction per Kill  | The amount of time taken off the Juggernaut's Kill button with each kill |     Time     |    2.5    |
| Can Vent                     | Whether the Juggernaut can vent                                          |    Toggle    |    ON     |
| Can Sabotage                 | Whether the Juggernaut can sabotage                                      |    Toggle    |    ON     |
| Impostor Vision              | Whether the Juggernaut has Impostor vision                               |    Toggle    |    ON     |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Marksman

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Receive A Longer Kill Distance With Each Kill<br>
__Win Condition__: Be The Last Player Alive<br>

`Originally Developed by Discussions`<br>
`Idea by WaW`<br>

#### Role Description
The Marksman gets a longer kill distance for each kill they make.<br>

### Game Options
|             Name               |                                 Description                            |     Type     |  Default  | 
| ------------------------------ | ---------------------------------------------------------------------- | :----------: | :-------: |
| Marksman                       | The probability of the Marksman appearing                              |  Percentage  |    0%     |
| Maximum                        | How many Marksmen should spawn                                         |    Number    |     1     |
| Kill Cooldown                  | The cooldown of the Marksman's Kill button                             |    Number    |  Global   |
| Kills Before Distance Increase | How many kills the Marksman needs before their kill distance increases |    Number    |    2      |
| Starting Kill Distance         | The kill distance that the Marksman begins with                        |    Number    |  Global   |
| Can Vent                       | Whether the Marksman can vent                                          |    Toggle    |    ON     |
| Can Sabotage                   | Whether the Marksman can sabotage                                      |    Toggle    |    ON     |
| Impostor Vision                | Whether the Marksman has Impostor vision                               |    Toggle    |    ON     |

_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_
_The Global option for Starting Kill Distance means that this setting will be the same as the Kill Distance in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Necromancer

__Faction__: The Undead<br>
__Base__: Impostor<br>
__Ability__: Convert Roles to the Undead<br>
__Win Condition__: Convert Roles to the Undead<br>

#### Role Description
The Necromancer is the main recruiter for the Undead faction. The first person it kills will become a Deathknight.<br>
With the help of the Deathknight, they must work together to convert others to the Undead.<br>
If the Necromancer were to die, The Deathknight would turn into Necromancer.<br>

#### Deathknight Role Description
The Deathknight must help the Necromancer convert players to the Undead. By using your pet button by someone who the Necromancer had used their kill button on, they will be converted.<br>
There can only be one Deathknight at a time, and if the Necromancer dies, the Deathknight will be the new Necromancer.<br>

### Game Options 
|             Name               |                                   Description                                 |     Type     |    Default    | 
| ------------------------------ | ----------------------------------------------------------------------------- | :----------: | :-----------: |
| Necromancer                    | The probability of the Necromancer appearing                                  |  Percentage  |      0%       |
| Maximum                        | How many Necromancers should spawn                                            |    Number    |       1       |
| Convert Cooldown               | The cooldown of the Necromancer's Kill button                                 |     Time     |      15s      |
| Immune to Partially Converted  | Whether the Necromancer is immune to attacks from partially converted players |    Toggle    |      ON       | 
| Deathknight                    | The options associated with Deathknight                                       |    Toggle    |     Show      |
| ┣ Can Become Necromancer       | Whether the Deathknight becomes the Necromancer upon death                    |    Toggle    |      ON       |
| ┣ Influence Cooldown           | The cooldown of the Deathknight's ability to convert players to the Undead    |     Time     |      5s       |
| ┣ Influence Range              | The distance the Deathknight needs to be from a player to convert them        |    Number    | Kill Distance |
| ┗ Influences Many              | Whether the Deathknight can influence many players at once                    |    Toggle    |      ON       |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Occultist

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Curse Players<br>
__Win Condition__: Curse & Kill Everyone & Be Last Player Alive<br>

#### Role Description
The Occultist's Kill/Curse Button alternates between cursing and killing players.<br>
Players will who are cursed by the Occultist will be seen with a cross during the meeting. If the Occultist is not voted off during this meeting, the cursed player dies.<br>
Regular kill self-reports Bait.\nSpell does not self-report Bait.<br>

### Game Options
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Occultist                    | The probability of the Occultist appearing                 |  Percentage  |    0%     |
| Maximum                      | How many Occultists should spawn                           |    Number    |     1     |
| Freely Switch Modes          | Whether Occultist can freely switch between Curse & Kill   |    Toggle    |    ON     |
| Switch Modes After Attack    | Whether Curse/Kill mode switches with each attack          |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Pelican 

<img align="right" width="" height="300" src="">

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Gulp Down the Competiton<br>
__Win Condition__: Gulp All Players For A Solo Win<br>

#### Role Description
The Pelican gulps players by using their kill button. Gulped players are teleported out of the map and are unable to interact with the game (including Sabotages). Upon a meeting being called, all gulped players will instantly die. If the Pelican dies or disconnects, all gulped players will return to where the Pelican last was.

### Game Options
|                 Name                   |                                     Description                                 |     Type     |  Default  | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :-------: |
| Pelican                                | The probability of the Pelican appearing                                        |  Percentage  |    0%     |
| Maximum                                | How many Pelicans should spawn                                                  |    Number    |     1     |
| Gulp Cooldown                          | The cooldown of the Pelican's Kill button                                       |    Number    |   Global  |
| Allow Escape from Pelican              | Allows players with teleportation abilities to teleport back onto the map       |    Toggle    |    ON     |

_The Global option for Gulp Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Plague Bearer

__Faction__: Neutral Killing <br>
__Base__: Impostor<br>
__Ability__: Infect Players & Become Pestilence<br>
__Win Condition__: None (must become Pestilence)<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Use the Kill button to infect everyone. Once everyone is infected, the Plague Bearer turns into Pestilence.

### Pestilence

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Immune To (most) Attacks<br>
__Win Condition__: Kill Everyone & Be The Last Player Alive<br>

#### Pestilence Role Description
Plague Bearer becomes Pestilence when they finish infecting all players. Pestilence cannot be killed (for the most part). Anyone who tries to kill the pestilence will backfire instead. Pestilence can be voted off or killed indirectly (like Warlock or Puppeteer).

### Game Options
|          Name             |                            Description                             |     Type     |  Default  | 
| --------------------------| ------------------------------------------------------------------ | :----------: | :-------: |
| Plague Bearer             | The probability of the Plague Bearer appearing                     |  Percentage  |    0%     |
| Maximum                   | How many Plague Bearers should spawn                               |    Number    |     1     |
| Infect Cooldown           | The cooldown of the Plague Bearer's Kill button                    |    Number    |  Global   | 
| Pestilence                | The options associated with Pestilence                             |    Toggle    |   Show    |
| ┣ Kill Cooldown           | The cooldown of Pestilence's Kill button                           |    Number    |  Global   |
| ┣ Unblockable Kill        | Whether Pestilence's kill can break through shields (e.g. Phantom) |    Toggle    |    OFF    |
| ┗ Invincibility Settings  | Whether Pestilence is invincible from player's attacks             |    Toggle    |    ON     |

_The Global option for Infect Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_
_The Global option for Kill Cooldown means that this setting will be the same as the Kill Cooldown in Custom Settings from vanilla Among Us_

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Retributionist

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Get A Second Chance At Living
__Win Condition__: Be The Last Player
 Alive<br>

#### Role Description
The Retributionist is a Neutral Killer with a twist. If the Retributionist were to ever die, It would have x seconds (Time configured by Host) to find their killer and kill them to come back to life. the Retributionist can come back multiple times, depending on host's settings.

### Game Options
|            Name              |                               Description                               |     Type     |  Default  | 
| ---------------------------- | ----------------------------------------------------------------------- | :----------: | :-------: |
| Retributionist               | The probability of the Retributionist appearing                         |  Percentage  |    0%     |
| Maximum                      | How many Retributionists should spawn                                   |    Number    |     1     |
| Revenge Time Limit           | The amount of time the Retributionist has to find and kill their killer |     Time     |    10s    |
| Invisible During Revenge     | Whether the Retributionist is invisible during revenge period           |    Toggle    |    OFF    |
| Number of Revenges           | How many times the Retributionist can seek revenge on their killer      |    Number    |     ∞     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## The Glitch

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Shapeshift & Roleblock Players<br>
__Win Condition__: Be The Last Player Alive<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Use the Kill button to Hack or Kill players. The Pet button can be used to switch between hacking and killing. Hacking prevents a player from using their buttons (report, vent, kill, sabotage).

### Game Options
|            Name              |                          Description                       |     Type     |    Default    | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-----------: |
| Glitch                       | The probability of the Glitch appearing                    |  Percentage  |      0%       |
| Maximum                      | How many Glitches should spawn                             |    Number    |       1       |
| Hacking Duration             | The amount of time a player is hacked                      |     Time     | Until Meeting |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Werewolf

__Faction__: Neutral Killing<br>
__Base__: Impostor<br>
__Ability__: Rampage: Kill With A Shorter Kill Cooldown<br>
__Win Condition__: Be The Last Player Alive<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Use Pet button to begin a rampage and kill with a shorter Kill Cooldown.<br>
NOTE: Werewolf can only kill during rampage!<br>

### Game Options
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Werewolf                     | The probability of the Werewolf appearing                  |  Percentage  |    0%     |
| Maximum                      | How many Werewolfs should spawn                            |    Number    |     1     |
| Rampage Kill Cooldown        | The cooldown of the Werewolf's Kill button during rampage  |     Time     |    1s     |
| Rampage Cooldown             | The cooldown of the Werewolf's rampage ability             |     Time     |    5s     |  
| Rampage Duration             | The duration of the Werewolf's rampage ability             |     Time     |    5s     |
| Can Vent Normally            | Whether the Werewolf can vent                              |    Toggle    |   OFF     |
| ┗ Can Vent in Rampage        | Whether the Werewolf can vent during rampage               |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Neutral Passive 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Amnesiac

__Faction__: Neutral Passive<br>
__Base__: Impostor<br>
__Ability__: Report a Body and Join Their Team<br>
__Win Condition__: Wins With The Team They Joined Or Crewmates (if chosen)<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description

The Amnesiac reports a body to join the player's team.<br>

If `Steals Exact Role` is OFF then the Amnesiac becomes:

 Neutral Killer = Hitman<br>
 Neutral Passive = Opportunist<br>
 Crewmate = Sheriff<br>
 Else (e.g. Impostor Madmate, etc.) = Jester<br>

### Amalgamation

__Faction__: Neutral Passive<br>
__Base__: Impostor<br>
__Ability__: Report a Body and Gain Their Abilities<br>
__Win Condition__: Determined In Settings<br>

`Idea by Town of Us Reactivated`<br>

#### Amalgamation Role Description 
The Amalgamation gains (becomes) the abilities of every player they report.<br>

### Game Options
|            Name              |                                  Description                              |     Type     |   Default   | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :---------: |
| Amnesiac                     | The probability of the Amnesiac appearing                                 |  Percentage  |     0%      |
| Maximum                      | How many Amnesiacs should spawn                                           |    Number    |      1      |
| Steals Exact Role            | Whether the Amnesiac commandeers the exact role of the player they report |    Toggle    |     OFF     |
| Has Arrows to Bodies         | Whether the Amnesiac has arrows to reportable bodies                      |    Toggle    |     ON      |
| Amalgamation                 | The probability of Amalgamation appearing                                 |  Percentage  |     0%      |
| ┣ Has Arrows to Bodies       | Whether the Amalgamation has arrows to reportable bodies                  |    Toggle    |     OFF     |
| ┣ Win Condition Determiner   | What role determines the Amalgamation's win condition                     |    Toggle    | Oldest Role |
| ┣ Max Absorbed Roles         | The max number of roles the Amalgamation can gain                         |    Number    |      ∞      |
| ┗ Absorb Modifiers           | If the Amalgamation also gains the modifiers (Oblivious is banned)        |    Toggle    |     OFF     |    

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Archangel

__Faction__: Neutral Passive<br>
__Base__: Engineer <br>
__Ability__: Protects Their Target <br>
__Win Condition__: Win With Their Target <br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description 
The Archangel’s Target is marked by a light blue diamond next to their name.<br>
Vent to temporarily protect your target from getting killed.<br>
If they win, you win.<br>				

### Game Options
|                Name                 |                              Description                          |     Type     |  Default  | 
| ----------------------------------- | ----------------------------------------------------------------- | :----------: | :-------: |
| Archangel                           | The probability of the Archangel appearing                        |  Percentage  |    0%     |
| Maximum                             | How many Archangels should spawn                                  |    Number    |     1     |
| Protect Duration                    | The amount of time the Archangel's Target is protected from kills |     Time     |   2.5s    |
| Protect Cooldown                    | The cooldown for the Archangel's Vent button                      |     Time     |   2.5s    |
| Target Knows They Have An Archangel | Whether the Archangel's Target knows they have a protector or not |    ON/OFF    |    ON     |
| Archangel Knows Target Role         | Whether the Archangel knows the role of their Target or not       |    ON/OFF    |    ON     |
| Role Change When Target Dies        | Role options for when the Archangel's target dies                 | Role Options |  Jester   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Copycat

__Faction__: Neutral Passive<br>
__Base__: Crewmate <br>
__Ability__: Copies Killer's Role When Killed<br>
__Win Condition__: Win's With Killer's Team<br>

#### Role Description
As Copycat, the first time you get attacked you'll change faction & role. If you were attacked by an impostor, you're now an impostor. If by a solo killer, then you're also a solo killer.<br>
Depending on the host's options, you may gain their 'progress' as well.

### Game Options
|                Name                 |                              Description                          |     Type     |  Default  | 
| ----------------------------------- | ----------------------------------------------------------------- | :----------: | :-------: |
| Copycat                             | The probability of the Copycat appearing                          |  Percentage  |    0%     |
| Maximum                             | How many Copycats should spawn                                    |    Number    |     1     |
| Copy Role's Progress                | Whether Copycat copies players progress (e.g. tasks completed)    |    Toggle    |    OFF    |
| Shapeshift Into Attacker            | Whether Copycat shapeshifts into their attacker                   |    Toggle    |    OFF    |
| Killer Knows Copycat                | Whether killer knows they've tried to kill the copycat            |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Executioner

__Faction__: Neutral Passive<br>
__Base__: Crewmate <br>
__Ability__: None <br>
__Win Condition__: Get Target Voted Off To Win<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Executioner’s Target is marked with a black name & win if their target is voted out.<br>
If the target dies before being voted out, the Executioner changes their Role and becomes Crewmate, Jester, or Opportunist according to a game option.<br>
If the target is the Jester, the Executioner can be an additional winner.

### Game Options
|            Name              |                             Description                            |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------ | :----------: | :-------: |
| Executioner                  | The probability of the Executioner appearing                       |  Percentage  |    0%     |
| Maximum                      | How many Executioners should spawn                                 |    Number    |     1     |
| Can Target Impostors         | Whether the Executioner can have an Impostor as a target or not    |    ON/OFF    |    OFF    |
| Can Target Neutrals          | Whether the Executioner can have a Neutral role as a target or not |    ON/OFF    |    OFF    |
| Role Change When Target Dies | The role given to the Executioner when their target dies.          | Role Options |   Jester  |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Hacker

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: None <br>
__Win Condition__: Fix Sabotages to Win<br>

`Originally Developed by Discussions`<br>
`Idea by The Other Roles`<br>

#### Role Description
As a Hacker, your goal is earn a number of points by fixing sabotages.<br>
Has powers of Sabotage Master. Each sabotage fixed earns you one point.<br>
Hacker can be killed by Sheriff.<br>

### Game Options (incomplete)
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Hacker                       | The probability of the Hacker appearing                    |  Percentage  |    0%     |
| Maximum                      | How many Hackers should spawn                              |    Number    |     1     |
| Hacker Can Vent              | Whether Hacker can vent                                    |    Toggle    |    ON     |
| ┣ Vent Cooldown              | The cooldown of the Hackers Vent button                    |    Toggle    |    ON     |           
| ┗ Vent Duration              | The duration a Hacker can stay in the vent for             |    Toggle    |    ON     |
| Points Needed to Win         | The amount of points needed for solo win                   |    Toggle    |    ON     |      
| Fast Fixes Lights            | Whether Hacker can Fast fix lights                         |    Toggle    |    ON     |      
| Fast Fixes Reactor           | Whether Hacker can Fast fix Reactor                        |    Toggle    |    ON     |
| Fast Fixes Oxygen            | Whether Hacker can Fast fix Oxygen                         |    Toggle    |    ON     |
| Fast Fixes Comms             | Whether Hacker can Fast fix Comms                          |    Toggle    |    ON     |
| Fast Fixes Doors             | Whether Hacker can Fast fix Doors                          |    Toggle    |    ON     |
| Fast Fixes Crash Course      | Whether Hacker can Fast fix Crash Course                   |    Toggle    |    ON     |
| Fixing Doors Gives Points    | Whether fixing doors gives points                          |    Toggle    |   OFF     |

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Jester

__Faction__: Neutral Passive<br>
__Base__: Crewmate/Engineer<br>
__Ability__: Options For Impostor Abilities (Venting & Impostor Vision)<br>
__Win Condition__: Get Voted Off<br>

`Originally Developed by Town of Host`
`Idea by libhalt`

#### Role Description
Jester gets a solo win if they can be voted out.<br>
Troll players in meetings, act sus in game.<br>

### Game Options
|                  Name                  |                       Description                      |     Type     |  Default  | 
| -------------------------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Jester                                 | The probability of the Jester appearing                |  Percentage  |    0%     |
| Maximum                                | How many Jesters should spawn                          |    Number    |     1     |
| Has Impostor Vision                    | Whether Jester has Impostor vision or not              |    Toggle    |    ON     |
| Can Use Vents                          | Whether Jester can use vents or not                    |    Toggle    |    ON     |
| Can't Call Emergency Meetings          | Whether Jester can call Emergency Meetings             |    Toggle    |    OFF    | 
| Minimum Meetings Before Ability To Win | How meetings must pass before Jester can win           |    Number    |     0     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Opportunist

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: None<br>
__Win Condition__: Remain Alive Until Game End<br>

`Originally Developed by Town of Host`
`Idea by The Other Roles: GM Edition`

#### Role Description
Regardless of the game outcome, Opportunist wins if they survive to the end of the match.<br>

### Game Options
|            Name              |                          Description                       |     Type     |  Default  | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Opportunist                  | The probability of the Oppotunist appearing                |  Percentage  |    0%     |
| Maximum                      | How many Oppotunists should spawn                          |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Phantom

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: Unkillable & Cannot Be Voted Out Until Last Few Tasks <br>
__Win Condition__: Complete Tasks To Win <br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
The Phantom cannot die until a set number of tasks (predetermined by host in settings) have been completed.<br>
When they are on their final tasks, everyone gets an arrow pointing straight toward them.<br>
Kill the Phantom before they finish tasks to stop them.<br>

### Game Options (incomplete)
|               Name                |                                                 Description                                            |     Type     |  Default  | 
| --------------------------------- | ------------------------------------------------------------------------------------------------------ | :----------: | :-------: |
| Phantom                           | The probability of the Phantom appearing                                                               |  Percentage  |    0%     |
| Maximum                           | How many Phantoms should spawn                                                                         |    Number    |     1     |
| Immune to Range Interactions      | Whether the Phantom is immune to second-hand interactions from other roles (like a Firework)           |    Number    |     1     |
| Remaining Task Warning            | The amount of remaining tasks that will allow the Phantom to be targeted (i.e. killed/interacted with) |    Number    |     1     |
| Remaining Tasks for Targetability | The amount of remaining tasks that will trigger an alert to killers (arrow pointing to phantom)        |    Number    |     1     |
| Override Phantom's Tasks          | Options to customize Phantom's tasks                                                                   |    Toggle    |   OFF     |
| ┣ Allow Common Tasks              | Whether the Phantom will receive Common Tasks                                                          |    Toggle    |    ON     |
| ┣ Phantom Long Tasks              | How many Long Tasks will be assigned to the Phantom                                                    |    Number    |     5     |
| ┗ Phantom Short Tasks             | How many Short Tasks will be assigned to the Phantom                                                   |    Number    |     6     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Postman 

__Faction__: Neutral Passive<br>
__Base__: Crewmate <br>
__Ability__: Deliver Messages To Other Players <br>
__Win Condition__: Deliver All Messages & Avoid Getting Voted Out <br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description (incomplete)
Complete tasks to receive Target information (arrows pointing to Target is an option for this role).<br>
Once Target is obtained (indicated by black name) Postman must deliver their message (touch the Target).<br>
Complete another task to get a new Target. Doing this before the last target's mail is delivered, results in suicide.<br>
The Postman will be revealed during the first meeting after they have completed deliveries to all living players.<br>
If the living players do not eject the Postman during this meeting, the Postman wins.<br>

### Game Options (incomplete)
|            Name              |                          Description                       |     Type     |     Default     | 
| ---------------------------- | ---------------------------------------------------------- | :----------: | :-------------: |
| Postman                      | The probability of the Postman appearing                   |  Percentage  |        0%       |
| Maximum                      | How many Postmen should spawn                              |    Number    |        1        |
| Has Arrow To Targets         | Whether Postman receives an arrow to it's targets          |    Toggle    |        ON       |
| When Target Dies             | Options for what happens when the Postman's target dies    |    Toggle    | Deliver To Body |
| Override Postman's Tasks     | Options to customize Postman's tasks                       |    Toggle    |       OFF       |
| ┣ Allow Common Tasks         | Whether the Postman will receive Common Tasks              |    Toggle    |        ON       |
| ┣ Postman Long Tasks         | How many Long Tasks will be assigned to the Postman        |    Number    |        5        |
| ┗ Postman Short Tasks        | How many Short Tasks will be assigned to the Postman       |    Number    |        6        |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Schrodinger's Cat

<img align="right" width="" height="300" src="">

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: Changes Affiliation When Attacked<br>
__Win Condition__: Wins With Faction They Convert To<br>

`Originally Developed by Discussions`<br>
`Idea by The Other Roles: GM Edition`<br>

#### Role Description
The Schrödinger's Cat changes their affiliation with each attack against them! Win with the faction you convert into, but be careful! Cats only have so many lives!

### Game Options
|                 Name                   |                                     Description                                 |     Type     | Default | 
| -------------------------------------- | ------------------------------------------------------------------------------- | :----------: | :-----: |
| Schrodinger's Cat                      | The probability of the Schrodinger's Cat appearing                              |  Percentage  |    0%   |
| Maximum                                | How many Schrodinger's Cats should spawn                                        |    Number    |    1    |
| Number of Lives                        | How many attacks the Schrodinger's Cat can receive before death                 |    Number    |    9    | 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Survivor 

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: Can Protect Self From Attacks<br>
__Win Condition__:Survive Until The End To Win<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Survive to the end to win. Use your Pet button to protect yourself from attacks for short period of time. Cannot win with Executioner or Jester.

### Game Options
|      Name      |                   Description                    |     Type     |  Default  | 
| -------------- | ------------------------------------------------ | :----------: | :-------: |
| Survivor       | The probability of the Survivor appearing        |  Percentage  |    0%     |
| Maximum        | How many Survivors should spawn                  |    Number    |     1     |
| Vest Duration  | The amount of time the Survivor is protected for |     Time     |   30s     |
| Vest Cooldown  | The cooldown for the Survivor's Vent button      |     Time     |   15s     |
| Vest Usages    | How many vests can be used by Survivor           |    Number    |    ∞      |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Terrorist 

Create and original idea by 空き瓶/EmptyBottle<br>

__Faction__: Neutral<br>
__Base__: Engineer<br>
Victory Conditions : Finish All Tasks, Then Die<br>

The Terrorist are the Neutral Role where they win the game alone if they die with all their tasks completed.<br>
Any cause of death is acceptable except vote.<br>
If they die before completing their tasks, or if they survive at the game end, they lose.<br>

__Faction__: Neutral Passive<br>
__Base__: 
__Ability__:
__Win Condition__:

`Originally Developed by 空き瓶/EmptyBottle`<br>
`Idea by Foolers Mod`<br>

#### Role Description
Finish all tasks and get killed to win. The Terrorist can also be voted out to win depending on host's settings.<br>

### Game Options
|            Name              |                      Description                       |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------ | :----------: | :-------: |
| Terrorist                    | The probability of the Terrorist appearing             |  Percentage  |    0%     |
| Maximum                      | How many Terrorists should spawn                       |    Number    |     1     |
| Can Win By Suicide           | Whether the Terrorist can win by suicide or not        |    Toggle    |    OFF    |
| Override Terrorist's Tasks   | Options to customize Terrorist's tasks                 |    Toggle    |    OFF    |
| ┣ Allow Common Tasks         | Whether the Terrorist will receive Common tasks        |    ON/OFF    |    ON     |
| ┣ Terrorist Long Tasks       | How many Long Tasks will be assigned to the Terrorist  |    Number    |     5     |
| ┗ Terroris Short Tasks       | How many Short Tasks will be assigned to the Terrorist |    Number    |     6     |
| Can Win By Exile             | Whether the Terrorist can win by Exile                 |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Vulture

__Faction__: Neutral Passive<br>
__Base__: Crewmate<br>
__Ability__: Can Make Bodies Unreportable<br>
__Win Condition__: Eat Bodies To Win<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Use the Report button to eat dead bodies and make them unreportable. The vulture can switch between eating bodies and reporting them using the Pet button.<br>
The Vulture wins when they've eaten a set amount of bodies, and they may also have an arrow pointing to dead bodies if enabled by host.<br>

### Game Options
|               Name              |                          Description                       |     Type     |  Default  | 
| ------------------------------- | ---------------------------------------------------------- | :----------: | :-------: |
| Vulture                         | The probability of the Vulture appearing                   |  Percentage  |    0%     |
| Maximum                         | How many Vulture should spawn                              |    Number    |     1     |
| Required Bodies                 | Amount of bodies needed for solo win                       |    Number    |     3     |
| Has Impostor Vision             | Whether the Vulture has Impostor vision                    |    Toggle    |    ON     |
| Can Switch Between Eat & Report | Whether the Vulture has the ability to report dead bodies  |    Toggle    |    ON     |
| Can Use Vents                   | Whether the Vulture can use vents                          |    Toggle    |    ON     |
| Has Arrows to Bodies            | Whether the Vulture has arrows to dead bodies              |    Toggle    |    ON     |
  
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Modifiers

## Bait

__Indicator__: Cyan ★

`Originally Developed by Discussions`<br>
`Idea by The Other Roles`<br>

#### Role Description
When Bait is killed, the impostor will automatically self report.<br>

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Bair                         | The probability of the Bait modifier appearing                            |  Percentage  |    0%     |
| Maximum                      | How many Bait modifiers should spawn                                      |    Number    |     1     |
| Restricted to Crewmates      | Whether the Bait modifier is restricted to Crewmates                      |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Bewilder

__Indicator__: Brown ⁂

`Originally Developed by Discussions`<br>
`Idea by Mek`<br>

#### Role Description
When someone with Bewilder is killed, they force the killer to have crew vision distance for the rest of the game.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Bewilder                     | The probability of the Bewilder modifier appearing                        |  Percentage  |    0%     |
| Maximum                      | How many Bewilders modifiers should spawn                                 |    Number    |     1     |
| Restricted to Crewmates      | Whether the Bewilder modifier is restricted to Crewmates                  |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Bloodlust

__Indicator__: Gradient Role Name

#### Role Description
The Bloodlust modifier allows the user to keep the ability of their role, while also giving them the ability to kill. Kill all other players to win.

### Game Options
|             Name               |                                  Description                              |     Type     |  Default  | 
| ------------------------------ | ------------------------------------------------------------------------- | :----------: | :-------: |
| Bloodlust                      | The probability of the Bloodlust modifier appearing                       |  Percentage  |    0%     |
| Maximum                        | How many Bloodlust modifiers should spawn                                 |    Number    |     1     |
| Restricted to Crewmates        | Whether the Bloodlust modifier is restricted to Crewmates                 |    Toggle    |    OFF    |
| Restricted to Compatible Roles | Whether the Bloodlust modifier is restricted to compatible roles          |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Deadly

__Indicator__: Green 乂<br>

#### Role Description
Players with the deadly modifier have their kill cooldown reduced by a set percentage.<br>

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Deadly                       | The probability of the Deadly modifier appearing                          |  Percentage  |    0%     |
| Maximum                      | How many Deadly modifiers should spawn                                    |    Number    |     1     |
| Cooldown Reduction           | The percentage the player's kill cooldown is reduced                      |  Percentage  |    25%    |
| Assignable to Non-Killing    | Whether Deadly can be assigned to Non-Killing roles                       |    Toggle    |    ON     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Diseased 

__Indicator__: Green §<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Multiplies the killer's kill cooldown upon death.<br>

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Diseased                     | The probability of the Diseased modifier appearing                        |  Percentage  |    0%     |
| Maximum                      | How many Diseased modifiers should spawn                                  |    Number    |     1     |
| Restricted to Crewmates      | Whether the Diseased modifier is restricted to Crewmates                  |    Toggle    |    OFF    |
| Cooldown Increase            | The percentage the killer's kill cooldown is increased upon death         |  Percentage  |   100%    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Flash

__Indicator__: Yellow ◎ <br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
The Flash makes the player move faster.<br>
Due to technical limitations, flash moves at normal speed for other players, and flash sees other players moving at the speed of Flash.<br>

### Escalation

__Indicator__: Gold ◉ <br>

`Originally Developed by Discussions`<br>
`Idea by Det`<br>

#### Role Description
Players with the Escalation modifier gain a static speed boost per kill.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Flash                        | The probability of the Flash modifier appearing                           |  Percentage  |    0%     |
| Maximum                      | How many Flash modifiers should spawn                                     |    Number    |     1     |
| Speed Increase               | The increase in speed granted to the Flash                                |    Number    |   0.25    |
| Escalation                   | The probability of the Escalation modifier appearing                      |  Percentage  |    0%     |
| ┗ Additional Speed Per Kill  | The increase in speed granted per kill                                    |    Number    |   0.4     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Nimble

__Indicator__: Yellow ☁<br>

#### Role Description
Grants any role the ability to vent, if they weren't able to previously vent.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Nimble                       | The probability of the Nimble modifier appearing                          |  Percentage  |    0%     |
| Maximum                      | How many Nimble modifiers should spawn                                    |    Number    |     1     |
| Vent Cooldown                | The cooldown of the Nimble's Vent button                                  |     Time     |    40s    |  
| Vent Duration                | The duration Nimble can stay in a vent for                                |     Time     |   14.5s   |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Oblivious

__Indicator__: Maroon ?!<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Oblivious cannot report bodies.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Oblivious                    | The probability of the Oblivious modifier appearing                       |  Percentage  |    0%     |
| Maximum                      | How many Oblivious modifiers should spawn                                 |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Romantic

__Indicator__: Pink ♥<br>

#### Role Description
During the first meeting of the game, the Romantic MUST vote a player to become their partner (otherwise they'll die). Once a partner has been chosen, the Romantic can use their Pet Button to temporarily grant a shield to their partner. The Romantic wins if their partner wins (and is alive) at the end of the game. If their partner dies, the Romantic will transform into either the Vengeful Romantic or the Ruthless Romantic.

#### Vengeful Romantic Role Description
The Vengeful Romantic had their love stripped away from them. Their goal is to now hunt down their partner's killer and to kill them. The Vengeful Romantic may use either their Pet Button or Kill Button to kill another player. But, if they target an innocent player, the Vengeful Romantic will die from misfire. After successfully avenging their partner, the Vengeful Romantic regains its normal win 

#### Ruthless Romantic Role Description
The Ruthless Romantic doesn't care about anything anymore, and just wants everyone dead. They act as a normal neutral killer, winning by themselves. If player of this role was originally a crewmate, the pet button functions as their kill button with a `CD: Xs` indicator for kill cooldown.

### Game Options
|            Name              |                                          Description                                        |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------------------------- | :----------: | :-------: |
| Romantic                     | The probability of the Romantic modifier appearing                                          |  Percentage  |    0%     |
| Maximum                      | How many Romantic modifiers should spawn                                                    |    Number    |     1     |
| Restricted to Crewmates      | Whether the Romantic modifier is restricted to Crewmates                                    |    Toggle    |    OFF    |
| Notify Target of Romantic    | Whether the Romantic's target is notified of becoming their partner                         |    Toggle    |    ON     |
| Protection Cooldown          | The cooldown of the Romantic's shield                                                       |     Time     |     0s    |
| Protection Duration          | The duration of the Romantic's shield                                                       |     Time     |     0s    |
| Vengeful Romantic            | Displays options for Vengeful Romantic                                                      |    Toggle    |   Show    |
| ┣ Can Kill Bystanders        | Whether the Vengeful Romantic's attack kills a player that is not their partner's killer    |    Toggle    |    OFF    |
| ┣ Arrow To Killer            | Whether the Vengeful Romantic has arrows to their partner's killer                          |    Toggle    |    OFF    |
| ┗ Suicide After Revenge      | Whether the Vengeful Romantic dies after avenging their partner's death                     |    Toggle    |    OFF    |
| Ruthless Romantic            | The probability of the Ruthless Romantic modifier showing in place of the Ruthless Romantic |  Percentage  |    0%     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Sleuth

__Indicator__: Blue ○ <br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Use the report button to report a body. In meeting chat, the Sleuth will receive a message revealing the role of the dead player. Sleuth can only see the role of the dead player if they reported the body themselves.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Sleuth                       | The probability of the Sleuth modifier appearing                          |  Percentage  |    0%     |
| Maximum                      | How many Sleuth modifiers should spawn                                    |    Number    |     1     |
| Restricted to Crewmates      | Whether the Sleuth modifier is restricted to Crewmates                    |    Toggle    |    OFF    |
 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Tiebreaker

__Indicator__: Purple ※<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
If there is a tie between two players in a meeting, the Tiebreaker's vote will decide who to eject or to skip.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Tiebreaker                   | The probability of the Tiebreaker  modifier appearing                     |  Percentage  |    0%     |
| Maximum                      | How many Tiebreaker modifiers should spawn                                |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Torch

__Indicator__: Peach ☀<br>

`Originally Developed by Discussions`<br>
`Idea by Town of Us Reactivated`<br>

#### Role Description
Torch is unaffected by lights out.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Torch                        | The probability of the Torch  modifier appearing                          |  Percentage  |    0%     |
| Maximum                      | How many Torch modifiers should spawn                                     |    Number    |     1     |
| Restricted to Crewmates      | Whether the Torch modifier is restricted to Crewmates                     |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Unstoppable

__Indicator__: Dark Maroon ◇ <br>

#### Role Description
Players with Unstoppable are able to kill through most types of protection, including Medic shields. Based on the host's options this may even include "pure" immunity such as the Phantom.

### Game Options
|            Name               |                                  Description                              |     Type     |  Default  | 
| ----------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Unstoppable                   | The probability of the Unstoppable  modifier appearing                    |  Percentage  |    0%     |
| Maximum                       | How many Unstoppable modifiers should spawn                               |    Number    |     1     |
| Can Kill Untargetable Players | Whether Unstoppable can kill unkillable roles                             |    Toggle    |    OFF    |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Watcher 

__Indicator__: Gray ▲<br>

`Originally Developed by Discussions`<br>
`Idea by The Other Roles: GM Edition`<br>

#### Role Description
Can see everyone's votes in meetings.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Watcher                      | The probability of the Watcher modifier appearing                         |  Percentage  |    0%     |
| Maximum                      | How many Watcher modifiers should spawn                                   |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Workhorse

__Indicator__: Green Θ <br>

#### Role Description
Gives even more tasks to a player.

### Game Options
|            Name              |                                  Description                              |     Type     |  Default  | 
| ---------------------------- | ------------------------------------------------------------------------- | :----------: | :-------: |
| Workhorse                    | The probability of the Workhorse  modifier appearing                      |  Percentage  |    0%     |
| Maximum                      | How many Workhorse modifiers should spawn                                 |    Number    |     1     |
| Restricted to Crewmates      | Whether the Workhorse modifier is restricted to Crewmates                 |    Toggle    |    OFF    |
| Additional Short Tasks       | How many additional Short Tasks the Workhorse receives                    |    Number    |     1     |
| Additional Long Tasks        | How many additional Long Tasks the Workhorse receives                     |    Number    |     1     |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
