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

1. **Item Name** - this is an unlabeled dropdown, but is self explanatory
2. **DIY Recipe** - if you set **Item Name** to "DIY recipe" this dropdown will appear.  It is also unlabeled, but self explanatory
3. **Count** - the item count has two distinct meanings:

  * For **stackable** items (materials, Nook Miles Tickets, ...) the count is the stack size **minus one**

    * This means that for a stack of 10 NMTs, you would set count to 9.  For 1 item, you would set count to 0
    * If you try to set count higher than it can go for a certain item (e.g. 99 NMTs) then in-game you will only have 1

  * For **non-stackable items with variations** (furniture, clothing, ...) the count is the index of the variations

    * NHSE may or may not tell you what variety corresponding to the count value
    * You can use either VillagerDB or the ACNH Data Spreadsheet to figure out which variation is which count value

4. **Uses** - the number of times the item has been used.  This field should *only* be used for breakable tools
5. **Flag0** - the first flag for the item.  For the purposes of basic item editing, this should be left as 0
6. **Flag1** - the second flag for the item.  For the purposes of basic item editing, this should be left as 0.

  * This option may disappear after selecting an item name

7. **Wrapped** - this checkbox may appear after selecting an item, and indicates whether or not the item is wrapped
8. **Wrapping Type** - this dropdown appears after checking the **Wrapped** option and indicates how it is wrapped (present or paper)
9. **Wrapping Color** - this dropdown appears if **Wrapped** is checked and **Wrapping Type** is set to 'WrappingPaper' and indicates the color of the wrapping paper
10. **Show Item Name** - this checkbox appears after checking the **Wrapped** option, presumably shows the item name before it is unwrapped

