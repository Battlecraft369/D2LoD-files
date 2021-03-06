## Hero Editor v.1.04 - edit characters for Single Player mode

---

- this version doesn't need install.
- download [HeroEditor104.zip](https://github.com/blizzhackers/D2LoD-files/raw/master/HeroEditor/HeroEditor104.zip) it anywhere you want on your PC.
- if you get errors about the *.ocx files missing, run **! register_ocx.bat** file
- before changing the **...\Hero Editor** folder location, run **! unregister_ocx.bat** file

- run Hero Editor.exe

![hero editor](HeroEditor.v104.png)

---

## How to Use Hero Editor

written mainly by Shokaku and ZonFire99 (www.ladderhall.com or www.ladderhallrealm.com)


List of Contents
----------------------------------
1. Getting Started
2. Editing Basic Stats
3. Editing Your Items
3.1 Adding an Attribute
3.2 Adding States Such As Invisibility
3.3 Setting Item Quality
3.4 Personalizing an Item
3.5 Creating an Item
4. Adding And Filling Sockets
5. Upgrading Your Weapons
6. Other Editing
6.1 Converting 1.09 Characters
6.2 Converting 1.09 Items
7. Getting Set Magic Working
8. Recovering Character Backups
9. Boss & Critter Powers (hexing)
10. Shortcuts to Menu Items
11. Tips


1. Getting Started

Download Hero Editor V1.04 Complete Install (see topic in the "Downloads" forum at www.ladderhall.com or www.ladderhallrealm.com). Unzip the downloaded file into a new (or at least empty) directory, and there should be three files ("setup.lst", "setup.exe", "Hero Editor.CAB"). Run (double click) the"setup.exe" file (or just "setup", if you have known file extensions hidden), and follow the directions (Click on the big button, on the left side). BTW, if a message comes up re "Version Conflict", answer yes (to keep the newer file that you already have).

Hero Editor usually requires that you are using an English version of Windows and your computer is set for single byte letters/Unicode, NOT multiple byte letters/UniCode.  (NOTE: I have never had this problem, but others tell me this solved the problem for them.)  From your Control Panel (Start > Settings > Control Panel) run Regional Settings, look for something about Unicode. Make sure the Unicode setting is for single bytes.  Also (MOST IMPORTANT for Win XP/Vista) make sure that you have the language setting for English (in BOTH the Regional Options tab, and the Advanced tab). If using WinXP, it might also help to right-click on Hero Editor.exe, select Properties, and in the Compatibility tab, select Windows 95 mode. If NOT set correctly, you will probably get error messages such as "unknown stat found: 21".

Note: Click on the Info tab of the ZonFire99 Edition Hero Editor to see what version is running, or look at the bottom-left of the main window.

If you have already installed a previous version of the Hero Editor but are having problems with missing or unregistered .ocx or .dll files, download Hero Editor V1.04 Complete Install, and these "missing" files will get automatically installed and registered.

Once installed, I suggest that you start the Hero Editor, click on Options tab, and make sure that you've selected 'Normal Error Response' as your Error Reporting and Response option (Option #2) as well as 'Rename and Keep All Backup Copies of Old Character Files' as your Automatic Character File Backup option (Option #7).

I also suggest that you completely segregate all old 1.03, 1.07, 1.09 and 1.10 items that you might have into a separate folder and then create a new folder for 1.11/1.12/1.13 items. Importing items from a different patch should usually not be done.  For example, importing 1.09 items into 1.10 or 1.11 characters can cause various problems and may even make your character unusable.  Similarly, there are 7 new items in 1.11 that can not be used in 1.10 games and characters.  1.03 items use a totally different item format and are never compatible with any other newer version.


2. Editing Basic Stats, V1.10 to 1.13

To edit your basic character stats, click on the Stats tab. Make any changes that you want as long as they stay within the maximums for Strength, Dexterity, Vitality, Energy, Life, Mana, Stamina, and Character Level.  Hero Editor will automatically limit the Stat values to be within the maximum values allowed by the D2 game.

Str/Dex/Vit/Energy max out at 1023
Life/Mana/Stamina max out at 8191
Character Level max out at 127

Note: While these are the maximum values that D2 LOD V1.10-1.13 will allow you to set in your character, you may exceed these values by adding item attributes that add or enhance the above stats (such as +nn to Life, +nn to Dexterity, etc.).  Using in-game editors can also allow you to increase these Stats when in a game, but the Stats will return to the above limits when the character file is saved.

NOTE:  You will need to visit Akara at the start of each game to "restore" your health and mana.  Also, the health and mana globes are only for display, and will not fill up properly when your health or mana goes over 32767.  But, this will have no effect on your actual health and mana -- they can still be much higher values.


3. Editing Your Items

To edit the magic attributes for an existing item in your char, click on the inventory tab, right-click on the item, and select "Specific Editing Functions" and "MAGIC Attribute Editing". In the Hero Editor Extras window, the Item Edit tab will be selected and three columns will appear. In the "Item Edit" column (left-most column), the item that you wanted to edit should be selected. In the middle column, the 'Magic' branch should be selected (click on it, if not) and the item's magic attributes should appear in the right-most column. 

NOTE:  If you want to edit items that are already socketed into this item, scroll down the "Item Edit" column (left-most column), and select one of the socketed items that are listed below this item.


3.1 Adding an attribute

1) To add a magic attribute to your item, right-click on the item, select ""Specific Editing Functions" and "MAGIC Attribute Editing". When the Hero Editor Extras window comes up, scroll the right-most, 'Magic Attribute' column to the bottom and click on "(1st empty slot)".

2) Now in the 'Magic Attribute' column (right-most column), there should appear a small scroll bar to the left of the top-most input box. Click on the down arrow to show the 'All Magic' tree.

3) Expand, contract, scroll up and down to select the attribute that you want to add.

To help you find things, attack, damage, defense, etc. attributes are generally where you might expect to find them (Any attributes that are not shown in the game are listed at the bottom in the 'NotVisible' branch).

Some special attributes such as magic-find, extra gold, increased sockets, replenish quantity, and requirements % can be found under the 'Extra' branch.

Some other special attributes such as chance of blocking %, indestructible, knock back, regenerate mana, replenish life, and throwable can be found under the 'Other' branch.

Some of the newest attributes for 1.10-1.13 are in the 'NotVisible' branch.

Once you've selected an attribute, the input box should shrink and show the default max value(s) for the attribute.

4) Set the value(s) to the desired amount(s) and click on the Save Modified Item button (below the middle column) to update your item.

5) To save your item in a file, go back to the Inventory tab, right-click on the item (look in the right-side window to see if the attributes are corrrect), and export your item.


3.2 Adding States Such As Invisibility

1) To add states to your item, right-click on the item, select "Specific Editing Functions" and "MAGIC Attribute Editing". When the Hero Editor Extras window comes up, scroll the right-most, 'Magic Attribute' column to the bottom and click on "(1st empty slot)".

2) Now in the 'Magic Attribute' column (right-most column), there should appear a small scroll bar to the left of the top-most input box. Click on the down arrow to show the 'All Magic' tree.

3) Scroll down and expand the 'NotVisible' branch.

4) Scroll down and select the "nv State" attribute (it is fourth from the bottom, unless your character is NOT a 1.10-1.13 character, then the "nv State" attribute will NOT appear at all). Now 2 pulldown boxes should appear--the first with "0 none" and the second with "1".

5) On the first pulldown box, open it and scroll to find the 'state' that you want. As an example, selecting '146 invis' will make you invisible to other players (but not monsters). Click on the Save Modified Item button (below the middle column) to update your item.

6) To save your item in a file, go back to the Inventory tab, right-click on the item (look in the right-side window to see if the attributes are corrrect), and export your item. 


3.3 Setting Item Quality

1) To set an item's quality, right-click on the item, select "Specific Editing Functions", select "Change the Item's QUALITY", and then select the desired quality.

2) At this point, the Hero Extras windows should appear and the specific qualities should be available for your choice in the right-most column (magical prefixes/suffixes, set names, unique names, rare/crafted prefixes/suffixes/name).

As an example, if you chose Unique, then the Hero Editor Extras window should show you all the unique qualities such as "the Gnasher", "Deathspade", "Bladebone", etc. in the right-most column.

3) Pick your specific quality and then click on the Save Modified Item button (below the middle column). As mentioned before, you can go back to the Inventory tab and export your item to save it in a file. 


3.4 Personalizing an Item

1) To personalize an item, select "Specific Editing Functions", select "PERSONALIZE (if possible)", and then select "Personalize Item".

2) When the Hero Editor Extras window appears, fill-in the desired name in the right-side input box.

3) Click on the Save Modified Item button (below the middle column) to update your item. As mentioned before, you can go back to the Inventory tab and export your item to save it in a file.


3.5 Creating An Item

1) To create a new item, click on the Extras button at the bottom of the main Hero Editor window.

2) On the Hero Editor Extras windows, click on the Item/Character Create tab.

3) Expand the All Items tree by clicking on the plus sign in front of the "All Items" and then expand Misc, Armor, or Weapons depending upon what type of item you wish to create.

4) Continue expanding sub-branches until you see and click the specific item that you wish to create. Depending upon the type of item, in the Description area, you may see damage (for weapons), one or more requirements and possibly the base number of sockets for the item.

5) Finally, go over to the right side of the window and click on the "Save New Item To PickedUp" button.

6) Returning to your inventory tab, right-click on an appropriate space for your item and right-click/paste the item where you want it. If you haven't already, go read the "'3. Editing Your Items"' section to add attributes and set item quality. 



4. Adding and Filling Sockets

To add empty sockets to an item, from the Inventory tab, right-click on the item and select "Specific Editing Functions", select "SOCKETING (if possible)" and then select "Make Item Socketed". This will add the Diablo II default max number of sockets for the item.

NOTE: To be able to use the 'base' number of sockets, the item will usually need to have a sufficiently high item level and quality.  By default, items are "now" created with a level of 90 (should be high enough).  But, by default, items are created with Superior quality, which may limit the maximum number of default sockets -- you may need to change the item quality to be Magical, Set, Rare, Unique or Crafted, to have all of the 'base' sockets available.

To add more empty sockets, in the Hero Editor Extras windows scroll down the middle column for the 'Magic' branch and add a new attribute 'Increased Sockets' and add the desired number of sockets (if you haven't already, go read the "3.1 Adding an Attribute" sub-section to add this atttribute).

When you add more empty sockets, please be aware that filling more than 7 sockets can caused instability problems for your character.  In the 1.10 patch, low, normal and superior items can only have 6 sockets, while magical, unique, rare, crafted and set items can have 7 sockets. Be sure to click on the Save Modified Item button (below the middle column) to save your changes.

To fill empty sockets with gems, jewels, or runes, simply drag and drop the gem/jewel/rune onto the socketed item. For example, from the inventory tab, click and hold a jewel in your inventory and move it on top of any item with an empty socket, then release the mouse button. Once a socket is filled, the additional attributes should be visible in the Description area to the right.  To fill all possible sockets with one item, make sure the item is in the Item Picked Up location, and then right-click on the item to be socketed and select Fill Item Sockets.

Note: After filling in 7 sockets on rings, the last jewel, gem, or rune seems to sometimes be ignored by D2. 


5. Upgrading Your Weapons

To change the item code for a weapon (or any other item), you must first copy the item to the Picked Up area (this is because the picture size might change, and not 'fit' in its original position). You can do this by right-clicking on the item and selecting "Copy Item (copy into Picked Up)", or simply click on the item to do a 'quick' copy. Now from the Picked Up area (move your cursor over the right side of the Inventory tab display), right-click on the item and select "General Edit of Item (in Extras Window)". In the Hero Editor Extras window, the Item Edit tab will be selected and three columns will appear. In the "Item Edit" column (left-most column), the item that you wanted to edit should be selected.

1) In the middle column, expand the 'Item Code' branch and select the 'Items Type Code' sub-branch. The individual item type codes and brief description should appear in the right-most column.

2) Scroll up or down and select the new item code that you want.

If you aren't sure what new item type code is better for your weapon (or any other item), click on the Item/Character Create tab and expand the All Items/Weapons branch/sub-branch (expand the other sub-branches for other type items).

Expand the sub-sub-branch for your weapon (in my case a bow) and click on the type of weapon that you have (say a "Short Bow"). In the description will appear the damage, one or more requirements and the base number of sockets for the item (in the case of a Short Bow, Two-Handed Damage; 1 to 4, Required Dexterity: 15, and Base number of 3 sockets).

Now select other weapons and look for the stats that you want. As an example, if I wanted to change my Short Bow to one that had the highest minimum 2-handed damage, I might choose a Diamond Bow because it has Two-Handed Damage: 33 to 40. Note that the item type code for a Diamond Bow (top of the right-hand side) is 6s7.

Now go back to the Item Edit tab, and scroll up or down the individual item type codes looking for 6s7 Diamond Bow (the items are sorted alphabetically, by their description). You can also search through the list by hitting the '6' key to cycle through all type codes that begin with '6', until '6s7' is found.  Select that item type code and click on the Save Modified Item button (below the middle column) to save your changes.

3) When you change an item type code, be sure to check the 'Number Of Sockets' sub-branch (under the 'Other' branch). In certain circumstances, the base number of sockets will be changed when you change the item type code, especially if you set the base number of sockets to less that maximum for the item.

Note: The Hero Editor will let you upgrade from any weapon to another weapon, from any armor item to another armor item, and from any misc item to another misc item. It will not let you convert across these three categories (such as upgrade from a weapon item to an armor item). 


6. Other Editing

If you look at the tabs on the main Hero Editor window, you will see that you can change Waypoints, Skills, Quests, Mercenary Experience and Introductions.

For edited characters, I usually enable all waypoints and set all quests to "Long Finished". I also usually set all skill levels to 99.  I tend not to bother with a mercenary nor introductions, but you can click on the appropriate tabs to make whatever changes that you desire.

When setting quests, it is best to make sure that the appropriate waypoints are also enabled, so I highly recommend enabling all waypoints all the time.


6.1 Converting Old Characters

The simplest way to convert an old character, such as 1.09 character to 1.13 format, is to open it with D2 LOD 1.13. Unfortunately, I've heard of various problems when trying to convert any high level character (character level above 99).

So I would recommend, editing your high-level chars with ZonFire99's Hero Editor and resetting the character level to 99 before opening your character with D2 LOD 1.13. Be aware that some conversion will occur right away and further changes will occur as you save and exit from a 1.13 game.

In particular, Str/Dex/Vit/Energy will be capped at 1023 and Life/Mana/Stamina will be capped at 8191 as you save/exit a game.

Also, certain 1.09-only attributes will be deleted. In my characters the old 1.09 Skill Level [1], [2], [3], etc. attributes disappeared. I've heard of others, but didn't get any details. All of my Unique items seemed to convert without any problems although the above Skill Level attributes did disappear. 


6.2 Converting Old Items

As mentioned elsewhere, you must strictly segregate your 1.03/1.07/1.09 items from your 1.10/1.11/1.12/1.13 format items. Do not import 1.09 items into your 1.13 chars--sometimes they work, sometimes there are minor problems, and sometimes it messes up your character.

So how do you convert your "great" 1.09 items that you spent all that time crafting?

1) You need to create a 'mule' character--dig out an old 1.09 char that is a teen or 99 (or go to the Extras window in the Hero Editor, click on the Item/Character Create tab, and click on the New V1.09D button to create a new 1.09 format character).

2) Set the level to 99. If you are using an existing character, delete items to create as much space as you need to import any 1.09 items that you want to convert, OR if you are creating a brand new character, just rename it to something appropriate.

3) Save the empty 'mule' character into both the Diablo II directory's \save sub-folder and a backup sub-folder.

4) Import all of your 1.09 items, save the character and use D2 LOD 1.11 to open the character.

5) If you haven't mixed anything up, D2 will convert your character (and all of its items) to 1.11 format.

6) Save and exit the game and then use the Hero Editor to open your converted 'mule' character.

7) Now you can export your converted items into your 1.11 items sub-folder and archive all of your 1.09 items.

If you haven't already, I strongly recommend that you take all of your old 1.09 items and move them to an archive folder that identifies them as 1.09 items (you might create a \109items sub-folder). 


7. Getting Set Magic Working

For each item in the Set that you are creating, perform the following steps:

1) If you haven't already, make sure that each item's quality has been properly specified as part of the desired set (see "3.3 Setting Item Quality" for an overview of how to set item quality).

2) From the inventory tab, right-click on each item, and select "Specific Editing Functions", select "SET Magic Editing", and then select "EDIT SET1 Magic Attributes". 

3) Click on the '(1st empty slot)' in the right-side, Set Magic Attributes area and add the desired attribute (see "3.1 Adding an Attribute" for step-by-step details on how to add an attribute).

4) Set the value(s) to the desired amount(s) and click on the Save Modified Item button (below the middle column) to update each item.

5) Repeat the above for adding additional Set Magic Attributes (i.e. Set 2, 3, 4, and 5).

NOTE: Unless you "know what you are doing", only put zero or one magic attribute in each Set Magic Attribute.  It is sometimes possible to put more than one, but you will often crash the D2 game when you 'mouse over' the Set item.

6) To save each item in a file, go back to the Inventory tab, right-click on each item (look in the right-side window to see if the attributes are corrrect), and export each item.

NOTE: The Set Magic Attributes will only be "available" if you have at least one more item in the Set equipped than the Set list number.  For example, if you have 5 'Set Magic Attributes' on an item (sets 1 to 5), but your character is only wearing 3 items, then only the first 2 Set Magic Attributes will be activated. These Set Magic Attributes will show up as green-colored magic attributes in the game.

BTW, the game also adds its own Magic Attributes for each Set as the Set is equipped (gold-colored magic attributes). The regular Magic Attributes show up as blue-colored magic attributes. 


8. Recovering Character Backups

If you have specified "Rename And Keep All Backup Copies of Old Character Files" as your "Automatic Character File Backup" option, then each time that you save your character file, a backup copy will be saved in the \save sub-folder of your Diablo II directory (the default path is C:\Program Files\Diablo II).

These backup files will use the following naming conventions: charnameDDHHMM.bak

where:
'charname' is the name of your character
'DD' .......... is the saved day of the month
'HHMM' ..... is the saved hour and minute

To recover one of these backup files, rename your current character file (.d2s suffix) out of the way and then rename the desired .bak file to your character file name (charname.d2s, where 'charname' is the name of your character).

NOTE:  If you do lots of editing to your character files, you may want to occasionally delete older .bak files that are no longer needed.

Once you are more familiar with editing character files, I recommend that you instead select "Keep Only One Backup File" or "Delete All Old Files".


9. Boss & Critter Powers (hexing)

First, put the desired non-class skill (such as "Baal Cold Missiles") on a charm -- don't add any skill bonus like 7 to all skills. Then, set the skill number on your right or left skill (or F1 key, etc.).  When you test this in a game, you won't see any skill icon there -- dont worry about it.  If you select any other skill while you are in the game you wont be able to select the monster skill again, unless you put the skill on one of the function keys (e.g. F1)

The "hexing" of the monster skill is done in Hero Editor by doing the following:

In the "Extras" window, select the "Character Hex" tab. Near the bottom-left, you will see Hotkey, Skill, and Side dropdown selections.  Select the Hotkey that you want to edit, such as <F1>.  Then select the Skill that you want assigned to the Hotkey, such as "318 Baal Cold Missiles".  You can then select the Side that you want for this Hotkey, either Right of Left.  If you have already made the charm, then Save, and you're done.

BTW, if you want to see the hex value for this skill, then on the list on the right side, scroll down and select "Skill ID Right Mouse", "Skill ID Left Mouse", or "64 Skill ID".  If you selected "64 Skill ID", the bytes on the left are for the F1 key, with the hex location starting at 56.  Each function key is allocated 4 bytes, even though only 1 or 2 are typcially used.  So, if you want to put the hex value for activation by the F2 key, put the hex value in at byte 60 (+61).  Similarily, move up another 4 bytes for F3, etc. for the rest of the function keys.  You can directly edit the hex values here if you desire.  For the above example, you should see "3E 01 00 00" in the location for <F1>.  The decimal value of 318, hex value 13E, gets stored in the character file hex as 3E 01, since the hex value of 13E needs to be "split" to fit in two bytes.


10. Shortcuts to Menu Items

The F1 key should always be "available" when you are doing anything in the main Hero Editor window.  Pressing the F1 key will use Notepad to open up a text description about how to use Hero Editor (i.e. this text description that you are reading now).

If the mouse cursor is over top of an item picture, the following shortcuts will also be available for that item:
<Ctrl>G will activate the Extras window, with the selected item ready for editing

<Ctrl>A will add all Magic Attributes for the selected item TO the Buffer
<Ctrl>P will pop up a window that lists all Magic Attributes that are presently in the Buffer
<Ctrl>B will delete all Magic Attributes presently in the Buffer
NOTE: Use the Extras window to paste all Magic Attributes FROM the Buffer into one of the Magic Attribute Lists for the selected item, either the Normal, Set1, Set2, Set3, Set4, Set5, or Runeword list.

<Ctrl>E will bring up the File Save dialog box to Export the selected item to a file
<Ctrl>I will bring up the File Open dialog box to Import an item from a file to the present location

<Ctrl>X will move the selected item to the "Picked Up" location
<Ctrl>C will put a copy of the selected item into the "Picked Up" location
<Ctrl>V will paste a copy of the "Picked Up" item into the present location
<Ctrl>Z will fill all available sockets of the selected item with copies of the item presently in the "Picked Up" location
Del will delete the item in the present location


11. Tips

1) When you put the mouse cursor overtop of an item picture, the 'Description' window to the right will list the name and properties of the item, and any Magic Attributes.  If the list is long, the text size will get smaller and the window will expand down to the bottom of the window.  If there are too many lines to fit on the displayed 'Description' window, then pressing the Up Arrow key will scroll the list up, so you can see additional lines (max 100 lines before 'errors' occur).  If you move the mouse, the list will reset to the 'top' of the list.  NOTE: The Diablo II game will usually "crash" if you have more than ~30 'visible' Magic Attributes on an item, which is easy to have on modified Set Magic items.

2) It is possible to make quick copies of an item.  First, click on the item, resulting in a copy of the item being placed in the 'PickedUp' location.  Then click on each of the locations you want a copy of the item.  This will quickly paste a copy of the item in the 'Picked Up' location.  You can also fill all unused areas with copies of the "PickedUp"location item.  TO do this, click the Paste All button below the "PickedUp" item picture.  This will work for the Person/Inventory, Stash, and Cube areas.

3) Holding the cursor stationary over certain locations will allow 'Tool Tip' text to appear.  This is a short description about additional features for this 'location'.  As an example, right-click on an item, select "Specific Editing Functions" and "MAGIC Attribute Editing". When the Hero Editor Extras window comes up, put the mouse cursor over the list of 'Magic Attributes' (the list on the right side).  You should see "Click to EDIT, <Shift>Click to DELETE, <Ctrl>Click to Add to BUFFER, <Alt>Click to Paste all from Buffer" pop up near the mouse cursor.  This same message will appear for Set and Runeword Magic attributes (which is the "only" way to quickly paste lots of Magic Attributes to Normal, Set and Runeword Magic attributes).

4) All of the Tree Views can be traversed using the mouse.  Also, most can be traversed using the keyboard too.  For example, the arrow keys can be used to expand and contract the branches, and to move up and down the list.  Also, you can 'jump' to certain list entries by pressing the first letter of the text description.  Pressing the same letter will cycle through the list entries that begin with that letter.  NOTE: Only entries in branches that have been expanded are used for this search.

5) There have been several changes to the items in the Options tab.  One recent addition is the "Search for D2 Directory" option.  It is now possible to tell Hero Editor to look for the D2 directory in the Registry either each time a character is opened (useful for D2GC, where this can often be changed), or only the very first time Hero Editor is started after installing Hero Editor.  Several less used options are now only located in the Hero Editor.INI file.  And some other new options have been added or features changed.
