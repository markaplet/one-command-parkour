# One Command Parkour System

A one command creation is a 100% vanilla minecraft command block contraption that adds or extends the functionality of Minecraft without the use of mods. What makes it a one command contraption is that all the command blocks are compressed into a single copy-paste command that once powered, the command block proceeds to build it's self and create the remaing command blocks used in the contraption.

## Parkour System

This contraption does not build a parkour course structure. Rather it only provides a base level scoring system, player checkpoint, teleportation on failure, and handful of other perks. It's up to your imagination in how you layout your course. Currently v1.0 offers only a handful features however, more features are planned so subscribe for updates.

## Game Setup

It seems that the currently popular trend in parkour is in a void world. While dropping players into the void is fun when it's not you being dropped into the void, it's less fun for players. This parkour system uses the minecraft:barrier block as a replacement for the void. When players fall from the course they land on the barrier block where they are teleported back to their last successful jump location. It's quick, it's painless, and more fun than spamming the respawn button.  

### Custom Flat world

Since this system relies on the barrier block, I recommend that you set up a new flat world with the following preset: **3;minecraft:barrier;127;** This will generate a flat world with only one layer of barrier blocks, thus giving you maximum build height and a foundation for which to build on without much effort.

### Give Command Block

For the sake of completeness, should you not be familiar with command blocks. Command blocks can only be obtained using the give command. In the chat type the following command **/give @p minecraft:command_block** If you are playing on a sever command blocks must be enabled in the server.properties file. You must also be in creative mode to access the GUI for the command block. If you need help, with this part, I would suggest going to YouTube and searching for something like "[command block give](https://www.youtube.com/results?search_query=command+block+give)"

### Install Command

Once you have your world created and a command block in hand, the installation is incredibly simple. Place down your command block in an area clear of the course (5 block radius). Then copy the [this](http://pastebin.com/raw/Gk4W9x2B) command into the command block and give it a signal. (button, redstone block, lever, etc) The contraption will build it's self before your very eyes like magic.

![](http://gph.is/1KjihQe)

### Constructing your course

The only rule to building a course is to ensure that any areas that players fall from contain barrier blocks below. Players do not have to fall on the 1 block layer as the floor of the world. You are free to build however you want, even if that is not a void. The only requirement is that in order to teleport a player, they must land on a barrier block. 

### Set Course Start/End

Attached to the front of the command block machine, there are two clickable signs to give yourself some spawn eggs for setting the start of the course and the end of the course. Use them at the appropriate locations to set the beginning and end of the course. 

### Carrot on a stick

If for any reason a player wishes to return to the beginnig of the course and start over, for example they may want to improve their score, or they are stuck for any reason, right clicking with the carrot on a stick will return the player to wherever you marked as the start of the course. 

## Single vs Multiplayer

version 1.0 has only tested this with single player, however the commands were written with multiplayer in mind, and should work fine. Because it has not been tested, it may have bugs. Consider it a warning. Feel free to post with  any issues discovered

## Updates

My plan for this tool is to update it with additional functionality and bug fixes as time allows. 

## Known Issues

The following are considered known issues and I am working on solutions. They were not IMO show stopping issues.

* Occasionally players will fall in an endless loop and forced to reset to the start of the course using the carrot on a stick.
* Occasionally the teleportation command will select the incorrect armor stand for the player and their position may be further back than they expected.
* If players render distance is set too short, for the course, they cannot teleport back to the start of the course. This is caused when the armor stand for the start of the course gets unloaded. The solution is to keep the course contained to a reasonable distance from the start of the course.
