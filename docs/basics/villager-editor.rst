.. NHSE Documentation:  Villager Editor Basics
   Basic usage of the villager editor.  Covers changing villagers,
   their houses, etc.

=======================
Villager Editor Basics
=======================

This section covers basic villager editing in NHSE - namely changing the villagers and their houses.

The Villager Editor
====================

The villager editor has several fields for each villager:

#. **Villager Index** - this is a 0-based index to determine which villager you're editing
   This only goes up to 9 (for 10 villagers)
#. **Species** - the species of this villager.  A table detailing the species IDs can be found below
#. **Variant** - the actual villager of the selected species.  This field is what distinguishes e.g. Bob from
   Lolly from Raymond

   * Trying to set this to an undefined/non-existent villager is neither tested nor recommended
   * You will see the name of the selected villager labeled to the right of the **Species** field

#. **Personality** - the personality of the villager

   * It is recommended that if you edit your villager, you also make their personality match what is expected
     in-game
   * Personality types can be found at either VillagerDB or the ACNH Data Spreadsheet

#. **Catchphrase** - the villager's catchphrase (e.g. "mochi" for Genji, "foxtrot" for Audie)

   * Clicking the **Original** button will fill in the villager's default catchphrase
   * A blank entry in this field is the same as having a default catchphrase

#. **Moving Out** - whether or not the villager is currently in boxes

   * Checking this box will show another dialog box regarding another flag to set - you should only follow the
     instructions if you actually want the villager to move out of your island.  If you just want to have them
     in boxes to give to others, the checkbox alone is enough

The Villager House Editor
==========================

The villager house editor can be found by clicking on the **Edit House** button in the **Villagers** tab.

Like the villager editor, there are several fields per villager that you can edit.  Ones of potential use
are listed below:

#. **<Wall|Roof|Door|OrderWall|OrderRoof|OrderDoor>UniqueID** - this determines the pattern used for the house

   * It is recommended (but not required) that you set these values to match the villager's correct house
   * If you are distributing this villager to others, please make sure it has the correct house!

#. **NPC1** - this is the **Villager Index** from the main villager editor corresponding to this list entry

   * e.g. if you have Raymond as villager index 0, then the 'Raymond's House' list item will have NPC1 set to 0

"Perfect" Villager Injection
=============================

The below is adapted from the `GBATemp tutorial on villager injection
<https://gbatemp.net/threads/tutorial-on-how-to-use-the-nhse-house-editor-for-perfect-villager-injection.563202/>`_.
The linked thread has an attachment which contains perfect, untouched villager and villager house files ready for you
to use in NHSE.  It is **strongly** recommended that you download this file pack to use for villager injection.

Following these steps with the above files will result in a clean, stock villager with the correct house:

#. Select the villager you wish to replace using the **Villager Index** field
#. Click **Load Villager**
#. Browse for and select the ``.nhv`` file for the villager you wish to injection
#. You will get a warning about the villager not originating from your data - click **Yes** to update the values

   * This will make the villager act as though they are from your island and not from the person who created the
     villager files

#. Save your save file in NHSE
#. Click **Edit House**.  The villager should already be selected
#. Click **Load**
#. Browse for and select the ``.nhvh`` file for the villager you injected
#. Click **Save**
#. Save your save file in NHSE

Villager Species IDs
==========================

The below table maps the villager species ID number to the "friendly" animal name (e.g. anteater, cat)

.. csv-table:: Villager Species ID Mapping
   :header: "Species ID", "Species Name"
   :align: center
   
   0, "Anteater"
   1, "Bear"
   2, "Bird"
   3, "Bull"
   4, "Cat"
   5, "Cub"
   6, "Chicken"
   7, "Cow"
   8, "Crocodile"
   9, "Deer"
   10, "Dog"
   11, "Duck"
   12, "Elephant"
   13, "Frog"
   14, "Goat"
   15, "Gorilla"
   16, "Hamster"
   17, "Hippo"
   18, "Horse"
   19, "Koala"
   20, "Kangaroo"
   21, "Lion"
   22, "Monkey"
   23, "Mouse"
   24, "Octopus"
   25, "Ostrich"
   26, "Eagle"
   27, "Penguin"
   28, "Pig"
   29, "Rabbit"
   30, "Rhino"
   31, "Sheep"
   32, "Squirrel"
   33, "Tiger"
   34, "Wolf"