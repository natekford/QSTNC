# QSTNC

Quickstack to Nearby Containers is inspired by Terraria's functionality of the (mostly) same name.

This is a mod for Fallout: New Vegas with the following dependencies: [xNVSE](https://github.com/xNVSE/NVSE/) and [JIP LN NVSE](https://www.nexusmods.com/newvegas/mods/58277). (It's been 9 months since I last looked at this code so there's a chance I'm forgetting a dependency, in which case it's some other mod that's included in TTW.)

The favorites system requires a background cell to store favorites (I'm sure there's some way to do this without actually creating anything in the GECK for the esp but I don't know how), if you want to compile this esp yourself you have to create a cell with 2 containers with the IDs `QSTNCFavoritesREF` and `QSTNCFavoritesInputREF`.

The esp file included in the scripts directory might work out of the box assuming the dependencies are installed?

The only way to invoke this esp's commands is via console. The following commands are the primary ones:

* `QSTNCStoreInventory` stores items from the players inventory into nearby containers that have the same items.

* `QSTNCFavoritesInput` opens a container that allows the player to put items in and count them as favorites (e.g. put 50 stimpaks in, stimpak count will not be quickstacked to below 50).