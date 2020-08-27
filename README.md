# Inferno Split Timer

### Overview
Inferno split timer displays the elapsed time to reach the following waves within the Inferno. 
The waves are generally accepted by the inferno community as the key milestones throughout the encounter.

* 9 - Melee 
* 18 - Ranger 
* 25 - Ranger + Melee
* 35 - Mager
* 42 - Mager + Melee
* 50 - Mager + Ranger
* 57 - Mager + Ranger + Melee
* 60 - Mager + Ranger + Melee + Blob
* 63 - Mager + Ranger + Melee + Blob(x2)
* 66 - Mager(x2)
* 67 - Jad
* 68 - Jad(x3)
* 69 - Zuk

### Info
This plugin does not perform the timing operation!

Inferno split timer relies on the infobox displayed by the newly added **Fight Caves and Inferno timers** plugin. Please make sure the following native runelite plugin is enabled:

* **Timers** -> **Fight Caves and Inferno Timers**

**NOTE:** The current **Fight Caves and Inferno Timers** plugin is currently off by 6 seconds. The plugin starts the timer once the `Wave: 1` message is displayed. This is incorrect. As stated by Mod Ash on twitter, the inferno timer starts when the player stands up from the "dropping in" animation. This is 10 ticks (6 seconds) before the `Wave: 1` message is displayed.

### How
For those curious. Here are the steps to taken by this plugin:

* Parse wave message to determine which wave the player is on
* If the player is on a split wave, the text displayed on the **Fight Caves and Inferno timers** plugin is parsed
* A chat message is displayed with the time parsed from the previous step

### Recognition
Special thanks to [@winterdaze](https://github.com/winterdaze) for doing all the hard work by implementing the tzhaar timers plugin into the base client.

