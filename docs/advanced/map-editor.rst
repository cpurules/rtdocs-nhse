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