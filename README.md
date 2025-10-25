# SECTION 1: EXECUTION & SYNTAX GUIDE
## Basic Info
#### Pro tip: Glacier has many similarities with "Adonis Admin", being heavily inspired by it.
The main way of executing commands with glacier is via the command bar, triggered by pressing right shift. Commands do not use a prefix.
## Player Selectors
Commands that accept players as an argument support a singular player or a comma separated list of player names.
#### Example: `kill player` *or* `kill player1,player2`
Note that player names are not case-sensitive and accept partial player usernames, however if multiple players match the partial, the command will not execute.  
  
In addition to using player names, Glacier also supports special identifiers for targeting certain group of players:

* `me` - yourself (executor of command)
* `all` - everyone in the server
* `others` - everyone in the server except yourself
* `admins` - all admins in the server (rank `moderator` or higher)
* `nonadmins` - everyone except admins (rank `moderator` or higher)
* `#NUM` - a select number of random people in the server
* `@USERNAME` - targets a player whose username matches exactly, case-insensitive
* `%TEAM` - targets players of a select team
* `radius-NUM` targets players within a certain radius around you (in studs) -- TO IMPLEMENT  
  
Placing `-` before any selector inverts the selection -- TO IMPLEMENT  
#### Example: `kill -radius-10` - kills all players further than 10 studs away from you
## Batch & Wait Commands
Commands can be ran sequentiually by using `//` between commands. --TO IMPLEMENT  
Additionally, you can also delay the execution of commands by using `wait NUM` --TO IMPLEMENT  
#### Example: `m Everyone will die in 10 seconds! // wait 10 // kill all` --Makes a message announcement, waits 10 seconds, and then kills everyone.
# SECTION 2: COMMAND USAGE
