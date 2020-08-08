.. NHSE Documentation:  Map Editor
   Covers topics related to the field item editor

=======================
Map (Field Item) Editor
=======================

This section covers topics related to map editing in NHSE.  This includes:

* Field items (adding/removing)
* Building manipulation (adding/moving/removing)
* Bridge/incline manipulation (adding/moving/removing)
* Terrain manipulation

To access the Field Item Editor, in the main NHSE window, go to the **Map** tab, click on **Edit Map...** and then
click on **Edit Field Items**.

**Note:**  It is recommended that you toggle on the 'Snap to nearest Acre on Click' option in the Field Item Editor.

Field Item Editing
==================

Field items are items (dropped, placed, planetd, etc.) on your island map.  The item editing functions can be found
in the **Items** tab in the Field Item Editor.

You can use the field item editor to do several item-related tasks, including:

* Add or remove a particular item to or from a particular tile on the map
* Bulk spawn items or DIYs
* Bulk removal from current acre or whole map
* Water all of your flowers

It is suggested that you read the :doc:`../basics/item-editor` documentation before continuing.

Per-Tile Item Editing
----------------------

Item editing on a per-tile basis functions very similarly to the inventory/storage editing functionality.  You
will see the item editor on the right.  You should make sure that the **Tile Editor Mode** option is set to
**Items**.

To **load** the item on a particular tile into the item editor, **left-click** the tile on the map preview.

To **clear** the item on a particular tile, **alt + left-click** the tile on the map preview.

To **set** the item on a particular tile to the item specified in the editor, **shift + left-click** the tile
on the map preview.

Alternatively, you can right-click the tile and choose **View** (load), **Set**, or **Reset** (clear).

Bulk Item Spawning
------------------

NHSE includes a basic bulk spawner that you can use to bulk-add items to your map.  To access the bulk spawner,
click on the **Remove Items...** button, and then click on the **Spawn...** option at the bottom.

The options available in the bulk spawner are as follows:

* **Spawn Type** (dropdown 1)

  * **ItemFromEditor** - bulk spawn the item currently loaded into the item editor
  * **SequentialDIY** - bulk spawn DIY recipes in sequential internal ID order

* **Spawn Layout** (dropdown 2)

  * **Square** - bulk spawns the item(s) in a square(ish) shape on the map
  * **Horizontal** - bulk spawns the item(s) in 2 rows on the map

* **X/Y** - the X/Y coordinate of the first item to spawn (upper-left coner for square layouts)
* **Count**

  * For **ItemFromEditor** spawn type, this is how many tiles to place the item/stack on
  * For **SequentialDIY** spawn type, this is how many of each DIY to generate

* **Start/Stop** (SequentialDIY only)

  * The (inclusive) start and end ID of the DIYs you wish to spawn

    * To spawn all DIYs, use the default of 0 to 9999; non-existent DIYs will not spawn
    * You can find resources with the DIY item IDs on the :doc:`../links` page

Bulk Item Removal
-----------------

NHSE provides functionality to bulk-remove items of a specific type (furniture, flowers, etc.) or of all types
from your map.

To access the bulk removal options, click on the **Remove Items...** button, and choose the type of item you
wish to clear from the map.  By default this will only remove items from the visible portion of the map.  To
remove the selected item type from the *whole* map, hold the **Shift** key while clicking the item type in the
button dropdown.

Flower Watering
----------------

NHSE provides functionality to automatically water all of the flowers on your map.

To access the flower waterer, click on the **Remove Items...** button and choose **Water Flowers**.  By default
this will only water flowers on the visible portion of the map.  To water flows on the *whole* map, hold the
**Shift** key while clicking the **Water Flowers** option in the button dropdown.

Building Manipulation
=====================

The list of buildings on your island, including the building options, is found on the **Buildings** tab of the
Field Item Editor.  You will see a list of the buildings and the map coordinates where they are placed.  Choosing
a building from the list will load the properties into the fields below (the Building Editor).

Buildings include actual buildings (resident services, Nook's Cranny, houses, etc.) as well as bridges and inclines.

Building Editor Fields
-----------------------

The following is a summary of the fields in the building editor and their purpose:

* **Building Type** - the type of building.  This is what distinguishes e.g. the museum from Nook's Cranny from a
  villager's house.  A mapping of the building IDs can be found at the end of this section.
* **X/Y** - the map coordinate of the building.  The origin (0, 0) of the map is the upper-left corner; that is,
  increasing Y will move the building towards the bottom of the map, and increasing X will move the building
  towards the right of the map
* **Angle** - the angle the building is placed at
  
  * This is only relevant for bridges and inclines; for actual buildings, it should be set to 0

* **Bit** - purpose unknown, recommended to leave at 0
* **Type** - the building subtype

  * This is only relevant for bridges and inclines, and determines what style of bridge/incline it is.  For actual
    buildings, it should be set to 0
  * Note that the same kind of bridge can have multiple subtypes; this is because bridges generally have a slightly
    different design based on how many tiles the bridge spans (4 v.s. 5)

* **TypeArg** - purpose unknown, recommended to leave at 0
* **UniqueID** - purpose unknown, recommended to leave at 0