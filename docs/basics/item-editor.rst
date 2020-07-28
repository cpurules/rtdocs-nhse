.. NHSE Documentation:  Item Editor Basics
   Basic usage of the item editor.  Covers commands, shortcuts,
   and non-flag edits

===================
Item Editor Basics
===================

This section covers basic item editing in NHSE - namely editing items in your inventory and in storage.

For information on editing the items on your map, check out the Field Item Editor guide.

The Item Editor
================

The item editor has several fields:

#. **Item Name** - this is an unlabeled dropdown, but is self explanatory
#. **DIY Recipe** - this is an unlabeled dropdown, but is self explanatory

   * This dropdown will only appear if **Item Name** is set to 'DIY recipe'

#. **Count** - the item count has two distinct meanings:

   * For **stackable** items (materials, Nook Miles Tickets, ...) the count is the stack size **minus one**

     * This means that for a stack of 10 NMTs, you would set count to 9.  For 1 item, you would set count to 0
     * If you try to set count higher than it can go for a certain item (e.g. 99 NMTs) then in-game you will only have 1

   * For **non-stackable items with variations** (furniture, clothing, ...) the count is the index of the variations

     * NHSE may or may not tell you what variety corresponding to the count value
     * You can use either VillagerDB or the ACNH Data Spreadsheet to figure out which variation is which count value

#. **Uses** - the number of times the item has been used

   * This field should *only* be used for breakable tools

#. **Flag0** - the first flag for the item

   * For the purposes of basic item editing, this should be left as 0

#. **Flag1** - the second flag for the item

   * For the purposes of basic item editing, this should be left as 0
   * This option may disappear after selecting an item name

#. **Wrapped** - indicates whether or not the item is wrapped

   * This checkbox only appears after selecting certain items

#. **Wrapping Type** - indicates how the item is wrapped (present, paper, or delivery)

   * This dropdown only appears after **Wrapped** is checked
   * The meaning of 'delivery' is not currently known

#. **Wrapping Color** - indicates the color of the wrapping paper

   * This dropdown only appears if **Wrapped** is checked and **Wrapping Type** is set to 'WrappingPaper'

#. **Show Item Name** - *presumably* shows the item name before it is unwrapped

   * Needs confirmation/testing
   * This dropdown only appears if **Wrapped** is checked

