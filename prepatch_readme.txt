Hearthstone Access community version
===================================

Contents
--------

- [01] Introduction
- [02] Changes to keyboard commands
- [03] How to install 
- [03a] Automated installation
- [03b] Manual installation
- [04] Known issues
- [05] Changelog
- [06] Contributing to development

Tip: You can easily jump to a section by searching for its number in this
document. For example to get to automated installation instructions search for
[03a].

[01] Introduction
-----------------

This document contains information about the community maintained version of
Hearthstone Access, a mod which makes Hearthstone accessible for blind players.
Hearthstone Access was originally developed by Guide Dev. After maintaining and
updating Hearthstone Access over a year Guide Dev announced that he was no
longer able to continue working on Hearthstone access. Developers from the
Hearthstone Access community were able to continue developing the mod after
Guide Dev provided some tools and information. To learn more about Guide Dev's
decision you can read his announcement about sunsetting Hearthstone Access
<https://hearthstoneaccess.github.io/sunsetting-hearthstone-access.html>

In addition to keeping up with updates to Hearthstone, the community developers
have added new features. Some notable updates include support for the new Death
Knight class, support for the remaining book of heroes and all of the book of
mercenaries solo adventures, support for the arena mode, and achievements. To
learn more about basics of Hearthstone Access you can visit its original web
site at <https://hearthstoneaccess.github.io/>.  Although Guide Dev no longer
maintains Hearthstone Access the web page still contains lots of useful
information like a basic introduction to the game, instructions how to install
the game and list of keyboard commands for Hearthstone Access.  The discord
server mentioned on the page is also still active and the best way to contact
the developers. So if you have suggestions or have found a bug the best place to
discuss those is the ask-the-developers channel on that discord server. You can
get to the server using this invite <https://discord.gg/WZWRenbuRe>

However notably the installation instructions for Hearthstone Access on the web
page do not work with this community version. Instead please use the
instructions in this document. This document also contains a section about known
issues, a changelog and information about how to contribute to the development
of Hearthstone Access.

[02] Changes to keyboard commands
---------------------------------

There have been some changes to keyboard commands that are not listed on the old
Hearthstone Access page.

- A and shift +a reads the number of corpses for the player and the opponent in
  addition to mana when the Death Knight class is used.
- When focused on your own minion you can use ctrl +f to have it attack the
  opponent's hero.
- F14 and F15 can be used to disable and enable accessibility. These are missing
  from most keyboards and are mainly Intendedto be used in for example
  autohotkey scripts that are used with Hearthstone Access.
- The R, A and O keys can be used in the main menu to quickly access play ranked, play casual and open packs respectively.
- While editing a deck in the collection manager, pressing space while focused on a card with a sideboard will open it.
- While opening a pack, the spacebar can now be used to reveal a random hidden card. This allows players to open packs much more quickly.

[03] How to install 
-------------------

Similar to original Hearthstone Access there are two ways to install: automated
and manual. Updating Hearthstone Access is also done using these same methods.
Notably Hearthstone Access has to be installed again every time Hearthstone
itself is updated. With minor Hearthstone updates, the same version of
Hearthstone Access usually works. But with more major updates changes are
required to Hearthstone Access itself before it works with the new version of
the game. Depending on the size of these changes and the availability of the
community developers, the update to Hearthstone access may take a varying amount
of time from just a couple of hours to a couple of days or even much longer in
rare cases.

### [03a] Automated installation

Community member leibylucw has developed a simple installation tool downloadable
via this link:
<https://github.com/leibylucw/hearthstoneaccess_beta_patcher/releases/download/v0.1.0/HearthstoneAccess_Beta_Patcher.exe>

After downloading the HearthstoneAccess_Beta_Patcher.exe program, move it to
your Hearthstone installation folder (in the file explorer press ctrl +x on it
and navigate to the game installation directory and press ctrl +v). By default
the installation directory is located at:  
C:\Program Files (x86)\Hearthstone  
Once the program has been moved execute it by pressing enter on it. A text
console window opens and you will see the following lines appearing one after
one after some delay:

    Downloading patch, please wait...
    Patching Hearthstone, please wait...
    Successfully patched!
    Press enter to exit the patcher.

After the final line appears you can press enter to quit the program. In the
future when ever you want to update or reinstall Hearthstone Access just run the
program again.

Note: when running the program for the first time you might encounter the
following error:

    Microsoft Defender SmartScreen prevented an unrecognized app from starting. Running this app might put your PC at risk.

If that happens select the More info  link and then press the run anyway button.

### [03b] Manual installation

You can always find the latest version of Hearthstone Access from here:  
<https://drive.google.com/file/d/1L6K6tVsXpFtPxUSgLTpxtNXVfN24Ym4l/view>  
Press the download button on that page to start the download.

In case you are already familiar with installing Hearthstone Access manually,
the process is the same just with the zip file from the link above. The bit
longer version is that you copy the contents of the patch folder inside the zip
file to your Hearthstone installation directory replacing any existing files
when prompted. By default this is  
C:\ProgramFiles (x86)\Hearthstone  

Below are more detailed instructions:

1. Navigate to the downloaded prepatch.zip and press enter on it.
2. You should now be inside the zip file (works at least on Windows 10 and
   later). There is a patch folder. Press enter on it.
3. You should now see three folders inside the patch folder: accessibility,
   hearthstone_data and strings. Press ctrl +a to select all of them and ctr +c
   to copy them to your clipboard.
4. Navigate to the Hearthstone installation folder which by default is:
   C:\Program Files (x86)\Hearthstone
5. Press ctrl +v to copy the files to the folder.
6. You will get a prompt informing you that the folder already contains some
   files with the same names and asking what do you want to do. Select the
   option Replace the files in the destination.
7. After the files have been copied Hearthstone Access has been installed
   successfully.

[04] Known issues
-----------------

Below are listed some known limitations or bugs of the current version of
Hearthstone Access.

- Some features related to the rune based deck building  of the Death Knight class are not yet supported. It is not currently possible to see or manually edit the rune composition of a death knight deck.
- In some cases involving discovering cards or drawing cards or otherwise adding
  extra cards to your hand during your turn, you might be prevented from playing
  a specific card you want or a wrong card is played instead.

### A note regarding unsupported modes

although most game modes are now fully supported, there still remain a few that have partial or no accessibility with the mod:

#### Mercenaries

 Blizzard has [announced](https://hearthstone.blizzard.com/en-us/news/23892226) that the mode will no longer get any new content. As such there are no plans to make it accessible at this time. You may be able to play using a combination of AutoHotkey scripts and GoldenCursor positions, which can be found on the Discord server.

#### Tavern Brawl

Work is currently under way to add accessibility for tavern brawls. Because the different weekly brawls involve slight variations on the user interface, some time will be required to ensure that they are all accounted for. It should be noted that once a match starts, it uses the same gameplay code as traditional Hearthstone, and as such is fully playable.

#### Solo adventures

The situation with older solo adventures is similar to that of tavern brawls, as they use different user interface variations and the games are fully playable once started. Support is planned. 

[05] Changelog
----------

### 2025-01-25

- Updated to Hearthstone 31.4.0.214839 (contributed by Endefx)
- If a player is building a starship, pressing A or shift+A will now announce the cost to launch it (contributed by Endefx)

### 2025-01-05

- The windfury and venomous effects on cards will now be read (contributed by Yncat)
- Fixed a bug where owners of the Battlegrounds season pass would be unable to claim any rewards past level 28 (contributed by Endefx)

### 2024-12-10

- Updated to Hearthstone version 31.2.0.213490 (contributed by Endefx)

### 2024-12-03 (2)

- Fixed an issue where spurious hero choices would appear for players without the season pass in Battlegrounds.

### 2024-12-03

- Updated to Hearthstone version 31.2.0.212197 (contributed by Endefx)
- The game startup sequence is now fully narrated (contributed by Endefx)
- Added support for the reroll mechanic in Battlegrounds. On the hero choice screen, press R to reroll the current hero, shift+R to reroll without confirmation, A to find out how many tokens you have. (Contributed by Endefx)

### 2024-11-04

- Updated to Hearthstone version 31.0.0.210640

### 2024-10-31

- Added support for the Great Dark Beyond pre-release tavern brawl (contributed by Endefx)
- Event weekly quests that are not yet active will now be properly read as such (contributed by Endefx)

### 2024-10-29

- Updated to Hearthstone version 31.0.0.210009 (contributed by Endefx)

Note that the new pre-release tavern brawl is not currently accessible. Support should be added in the next few days.

### 2024-10-13

- Players in China are now able to access the in-game shop (contributed by Endefx)
- Fixed some inaccessible popups that were appearing for Chinese players (contributed by Endefx)


### 2024-10-10

- Updated to Hearthstone version 30.6.0.208591 (contributed by Endefx)
- Fixed a bug that locked some players out of the arena (contributed by Endefx)

### 2024-09-10

- Updated to Hearthstone version 30.4.0.206605 (contributed by Endefx)

### 2024-08-21

- Fixed a hang caused by viewing the leaderboard while choosing a trinket in Battlegrounds (contributed by Endefx)

### 2024-08-20

- Updated to Hearthstone version 30.2.0.205267 (contributed by Endefx)
- It is now possible to read the cost of a minion on the board (contributed by Endefx)
- Added support for the new trinkets mechanic in Battlegrounds. While playing, press Q to view your trinkets, Shift+Q to view those of your opponent (contributed by Endefx)

### 2024-07-16

- Updated to Hearthstone version 30.0.0.203120 (contributed by Endefx)
- Improvements for the mod's handling of locations (all contributed by Endefx):
- - When a location is reopened or destroyed, this will now be narrated
- - When the opponent or spectated player plays a location, the full text is now read (the behavior now matches other card types)

### 2024-06-18

- Updated to Hearthstone version 29.6.0.201392

### 2024-06-17

- Updated to Hearthstone version 29.6.0.201108 (contributed by Endefx)
- The Dungeon Run and Monster Hunt adventures are now accessible (contributed by Endefx)
- Fixed an issue where health changes to heroes in Twist were not being reflected properly (contributed by Endefx)

### 2024-06-01

- Implemented full support for the "Whizbang’s Heroes" season in Twist (contributed by Endefx)
- The Battlegrounds rewards track is now accessible (contributed by KeyWasFull)
- You can now challenge your friends to tavern brawls (contributed by Mazen)
- On the tavern brawl screen, more information will now be provided such as your number of wins in the current brawl and the time until it ends (contributed by Mazen)

### 2024-05-17

- Updated to Hearthstone version 29.4.0.199503

### 2024-05-14

- Updated to Hearthstone version 29.4.0.198933 (contributed by Endefx)

### 2024-04-16

- Updated to Hearthstone version 29.2.0.198037 (contributed by Endefx)
- Players who have achieved the Legend rank can now read the rank of their opponent (contributed by Endefx)

Note: the newly launched Battlegrounds Duos mode is not accessible at this time.

### 2024-03-15

- Added support for upcoming Zilliax Deluxe 3000 and Splendiferous Whizbang cards (contributed by Endefx)
- Fixed a bug preventing dynamically updating card names from being read, which made the "Say my Name" tavern brawl unplayable (contributed by Endefx)
- The remaining turns in play of objectives and paladin auras will now be announced (contributed by Endefx)
- When a paladin aura or objective leaves play, this will now be announced (contributed by Endefx)
- Fixed a bug that caused an erroneous hero death announcement when a hero card was played (contributed by Endefx)

### 2024-03-11

- Updated to Hearthstone version 29.0.0.195635 (contributed by Endefx)
- When queueing for a match, you can now press space to announce the time you've spent in the queue as well as the estimated remaining time (contributed by Mazen)
- It is now possible to interact with recent players in the social panel (contributed by Endefx)

### 2024-02-02

- If an item in the shop can be bought for either gold or runestones, both options will now be offered (contributed by Endefx)
- Changed keyboard input handling to be more responsive and fixed an issue where modifier keys would have to be held longer than usual to be registered (contributed by Endefx)
- Resolved more instances of the issue causing cards to be read as "UNKNOWN ENTITY [cardType=INVALID]" (contributed by Endefx)
- In Battlegrounds, effects such as frozen and darkmoon tickets will now be read on tavern spells (contributed by Endefx)

### 2024-01-24

- Updated to Hearthstone version 28.4.0.192896

### 2024-01-18

- Updated to Hearthstone version 28.4.0.192412 (contributed by Endefx)
- Fixed an issue where multi-class cards would be read as neutral in some contexts (contributed by Endefx)
- Added a shortcut (T) to quickly access tavern brawl from the main menu (contributed by Endefx)

### 2023-12-24

- Updated HearthstoneAccess to support the new player experience (contributed by Endefx)
- Added support for the new catchup packs (contributed by Endefx)
- Fixed an issue that prevented players from entering the arena for the first time (contributed by Endefx)
- Added partial support for the tavern brawl mode (contributed by Endefx)

Known issue: HearthstoneAccess may lock up just after completing the apprenticeship. Restart the client to resolve this.

### 2023-12-09

- Updated the shop implementation for Hearthstone 28.2. Note that the shop layout has been completely redesigned, and now reflects the tabbed structure shown on- screen. (contributed by Endefx)

### 2023-12-06

- Updated to Hearthstone version 28.2.0.190416 (contributed by Endefx)
- Added support for the tavern spells mechanic in Battlegrounds (contributed by Endefx)

Warning! This update has introduced several major changes to the game. As a result, the shop will be temporarily inaccessible until we can account for the redesign.
In addition, the new player experience has been completely revamped. If you are still in the apprentice ranks, we recommend not to install this mod version as none of the new ui is accessible at this time.

### 2023-11-13

- Implemented the mass pack opening feature. To start, select a pack on the pack opening screen and press space. (contributed by Endefx)
- Fixed an issue where trying to open a pack that is locked, for example when it is part of a preorder, would cause a nonsensical string to be spoken (contributed by Endefx)
- The pack opening screen will once again automatically close after all packs have been opened (contributed by Endefx)


### 2023-11-09 (2)

- Updated to Hearthstone version 28.0.0.189384 (contributed by Endefx)

### 2023-11-09

- Disabled an inaccessible class unlock popup that recently started appearing for some players (contributed by Endefx)

### 2023-11-07

- Updated to Hearthstone version 28.0.0.189017 (contributed by Endefx)
- When reading your opponent's mana during gameplay, their current mana count will now be read along with the total amount (contributed by KeyWasFull)

### 2023-10-30

- Added accessibility for the new Hearthstone tutorial (contributed by Endefx)

Note: the skip tutorial button is currently inaccessible.

### 2023-10-17

- Updated to Hearthstone version 27.6.0.187190 (contributed by Endefx)
- Fixed an issue with choose one rewards where it was possible to claim an item that was already part of the player's collection, leading to unpredictable behavior (contributed by Endefx)

Warning! Blizzard has completely rewritten the Hearthstone tutorial in this version. If you are a new player, please wait for us to make it accessible with the mod.

### 2023-09-19 (2)

- Fixed a regression in Battlegrounds where pressing the O key would erroneously announce that there are no anomalies (contributed by Endefx)

### 2023-09-19

- Updated to Hearthstone version 27.4.0.185749 (contributed by Endefx)
- Added support for anomalies in traditional Hearthstone modes. The O key can be used to read them during gameplay. (contributed by Endefx)
- Added accessibility for the Battlegrounds collection manager. This currently supports hero skins, bartenders and strikes. (contributed by Endefx)

### 2023-09-06

- Updated to Hearthstone version 27.2.2.185054

### 2023-09-02
- When editing a deck in the collection manager, it is now possible to craft or disenchant the currently focused card by pressing Shift+Enter (contributed by Endefx)
- Restored the ability to change the format of a deck in the collection manager (contributed by Endefx)
- Fixed an issue in Battlegrounds where your final place would not be read in friendly matches and while spectating (contributed by Endefx)

### 2023-08-22

- Updated to Hearthstone version 27.2.0.183876 (contributed by Endefx)
- When using the T key to forge a card, this will now be correctly announced as forging (contributed by Yncat)
- When discovering a card, it is now possible to hide the discover interface using the tab key and inspect the game board (contributed by Endefx)
- Added an option to record textual logs of traditional Hearthstone games. Once enabled, the logs will be saved in a directory called "battle logs" found in the main Hearthstone directory (contributed by KeyWasFull)
- Added support for the new anomaly mechanic in Battlegrounds. They will be read along with the available tribes at the start of the game and when pressing the O key. (contributed by Endefx)

### 2023-08-01

- It is now possible to view multiple related cards in the collection manager (contributed by Endefx)
- Fixed an issue where pressing shift+F could cause a location such as Prison of Yogg-Saron to activate and target the enemy hero (contributed by Endefx)
- Twist will no longer be shown in the format picker menu when it is inactive (contributed by Endefx)

### 2023-07-25

- Updated to Hearthstone version 27.0.0.181554 (contributed by Endefx)
- Fixed an issue causing multi-target cards to erroneously present the discover interface in some cases (contributed by Endefx)
- Fixed an issue preventing the "Choose a target" prompt from being announced for additional targets of multi-target cards (contributed by Endefx)
- Fixed an issue where pressing the up and down arrow keys while choosing a target could skip over lines of the card being read (contributed by Endefx)


### 2023-07-11

- Fixed an issue causing a hang and reconnect in Battlegrounds on the 6 gold turn when quests are enabled (contributed by Endefx)
- Fixed an issue causing placeholders in Battlegrounds quest reward text to be read incorrectly (contributed by Endefx)

### 2023-06-28

- Updated to Hearthstone version 26.6.0.179020 (contributed by Endefx)
- Heroic duels are now accessible (contributed by Endefx)
- The new Twist mode is now accessible. See below for a known issue (contributed by Endefx)
- Arena and Duels will no longer appear in the modes menu if you haven't unlocked all classes (contributed by Endefx)

There are the following known issues in this version. They will be addressed in later updates:

- It is not currently possible to read the season rules for the Twist mode. For now, refer to the Twist announcement at <https://hearthstone.blizzard.com/en-us/news/23968054/introducing-hearthstone-s-new-mode-twist>.
- The ability to change the format of a deck in the collection manager has been temporarily disabled.

### 2023-06-10

- Added a workaround to prevent the mod from playing the wrong card in some rare cases (contributed by KeyWasFull)
- The Japanese language is now available (contributed by Yncat)

### 2023-05-31
- Updated to Hearthstone version 26.4.0.175913 (contributed by Endefx)

### 2023-05-22
- Various bug fixes and minor improvements for duels (contributed by Seva Popov, Nahana and Endefx)

### 2023-05-16
- The duels mode is now accessible. At the moment only casual duels are supported. (contributed by Seva Popov, Nahana and Endefx)

### 2023-05-10
- Updated to Hearthstone version 26.2.0.174258 (contributed by Endefx)
- It is now possible to read the list of members in a battlegrounds party (contributed by Endefx)
- Minions destroyed by Patchwerk in the hand will now be read (contributed by Endefx)


### 2023-04-10

- While opening a pack, the spacebar can now be used to reveal a random hidden card. This allows players to open packs much more quickly. (contributed by Endefx)
- It is now possible to change the format (standard/wild) of a deck while editing it in the collection manager. (contributed by Endefx)
- It is now possible to purchase packs in bulk with gold in the ingame shop (contributed by Endefx)

### 2023-04-04

- Updated to Hearthstone version 26.0.0.170824 (contributed by Endefx)
- Added an option to change the speed of minion attacks with shift+f. You will need to experiment with the different values to determine the one that is most suitable for your hardware and network. (contributed by KeyWasFull)
- Fixed an issue where pressing the escape key while in the sound options menu would erroneously open the game menu on top of it (contributed by Endefx)

### 2023-03-16

- It is now possible to read the quests on the event tab (contributed by KeyWasFull)
- Added a potential fix for the issue in Battlegrounds where the buddy button would not be read correctly in some cases (contributed by Endefx)
- In battlegrounds, the minion type of buddies will now be read on the hero choice screen and the buddy button (contributed by Endefx)

### 2023-03-15 (2)

- Added initial accessibility support for the event tab of the journal (contributed by KeyWasFull)
Fixed some issues with the adventure chooser (contributed by KeyWasFull)


### 2023-03-15

- Updated to Hearthstone version 25.6.0.168788 (contributed by Endefx)
- Buddies have returned to Battlegrounds! Press D to see the stats and current cost of your buddy, and enter to buy.
- The sideboard mechanic used by cards such as E.T.C., Band Manager is fully accessible. When editing your deck, focus on E.T.C. and press spacebar to see his band! (contributed by Endefx)
- The Knights of the Frozen Throne adventure is now accessible (contributed by KeyWasFull)
- Known issue: It is currently not possible to start the new event using the mod. We are working hard and hope to resolve this soon.

### 2023-03-11

- In option menus, the current value of checkboxes and dropdown controls will now be read (contributed by Endefx)
- Scrolling has been implemented in the social panel. You will now be able to interact with all of your friends. (contributed by Endefx)
- Fixed an issue that allowed the crafting button to be pressed even if there was not enough dust to craft the card (contributed by Endefx)
- Changed the reading of minion enchantments to be more reliable (contributed by Endefx)

### 2023-02-26

- Fixed an issue that caused the haunting of cards during gameplay to be read incorrectly (contributed by KeyWasFull)
- Fixed an issue with the accessibility of the new free deck claiming experience (contributed by Endefx)
- In the collection, the expansion or set that a card belongs to will now be read (contributed by Endefx)
- Modified the corpse counter to bring it in line with the changes in patch 25.4. See the Hearthstone patch notes for more information. (contributed by Endefx)
- It is now possible to replay and skip the traditional Hearthstone tutorial (contributed by Endefx)
- The new sound options menu is now accessible. Note that all options related to sound have moved into this menu. (contributed by Endefx)

### 2023-02-14

- Updated to Hearthstone version 25.4.0.165029 (contributed by Endefx)
- The revamped free deck experience for new and returning players is now accessible. You will be able to play with your loaner decks and claim them once the trial period expires. (contributed by Endefx)
- Cards haunted by the card "Haunting nightmare" will now be announced (contributed by KeyWasFull)
- In the options menu, it is now possible to disable speech while Hearthstone is in the background (contributed by KeyWasFull)

### 2023-01-29

- It is now possible to interact with missing and invalid cards while editing a deck (contributed by Endefx)
- Restored the original behavior of the tab key in some horizontal menus (contributed by KeyWasFull)
- Added three new shortcut keys to the main menu: R to play ranked, A to play casual and O to open packs (contributed by Saladeuh)
- Fixed an issue preventing players from starting their first arena run (contributed by KeyWasFull)

### 2023-01-23

- Updated translations
- Added a "Enable debug logging for this run" item to options. Developers may
  ask you to use this if you are reporting an issue. (contributed by KeyWasFull)
- Fixed an issue related to browsing coins in your collection (contributed by
  KeyWasFull)

### 2023-01-17

- Updated to Hearthstone version 25.2.0.162867 (contributed by Endefx)

### 2023-01-15

- Achievement fixes (contributed by  KeyWasFull)

### 2023-01-13

- It is now possible to view and claim achievements in the journal (contributed by  KeyWasFull)

### 2023-01-05

- Updated to Hearthstone version 25.0.4.162171 (contributed by Endefx)

### 2022-12-30

- Support for purchasing arena tickets with gold (contributed by  KeyWasFull)
- Support for reading of darkmoon tickets in Battlegrounds (contributed by  KeyWasFull)

### 2022-12-26

- Fixed a bug where increases to spell damage were being reported incorrectly (contributed
  by  Endefx)
- Updated translations
- Various improvements (contributed by  HLLF)

### 2022-12-23

- Fixed a bug where a popup dialogue related to the event rewards track prevented
  Hearthstone Access from working correctly (contributed by  Endefx)

### 2023-12-22

- Support for the arena mode (contributed by  KeyWasFull)
- Internal changes in how modifier keys (ctrl, shift, alt) are handled
  (contributed by  HLLF)
- f14 and f15 can be used to disable and enable accessibility (contributed by
  HLLF)

### 2022-12-17

- Updated translations
- It is no longer possible to access the emote menu when spectating (contributed by Mazen)
- More fixes to multi-target cards (contributed by  KeyWasFull)

### 2022-12-15

- Battlegrounds party announcements (contributed by  KeyWasFull)
- multi-target card fix (contributed by  KeyWasFull)
- It is now possible to purchase items in the ingame shop with runestones (contributed by  LordLuceus)

### 2022-12-12

- Battlegrounds invite changes  (contributed by  KeyWasFull)
- When choosing a deck to play, it is now possible to read the number of ranked wins with its class (contributed by  KeyWasFull)

### 2023-12-10

- Signature cards are now properly read as such (contributed by  HLLF)
- code cleanup (contributed by  HLLF)
- Added support for challenging friends to battlegrounds (contributed by
  KeyWasFull)

### 2022-12-09

- Restored the reading of rewards track XP (contributed by  Endefx)
- The card reroll popup is now accessible (contributed by  Endefx)

### 2022-12-08

- Reverted the quicker shift +f attack since it was unreliable for some users (contributed by
  Endefx)
- Made the Death Knight and Demon Hunter prologues accessible (contributed by
  KeyWasFull)
- Updated translations
- When reading your level in the rewards track, it is now possible to find out your current xp and the amount required for the next level (contributed by  Mazen)

### 2022-12-06

- Improved the Death Knight corpse counter (contributed by Alex19EP)

### 2022-12-04

- The attack speed when using shift +f is now faster (contributed by  KeyWasFull)
- Fixes to the end of game screen (contributed by  JScholes and HLLF)
- Fixed the handling of choose one hero powers used in some solo adventures (contributed by  KeyWasFull)
- Fixed the tracking of unlocked classes (contributed by  Endefx)

### 2022-12-02

- Fixed the spectate button in the social panel (contributed by  KeyWasFull)
- It is now possible to read the runes on Death Knight cards in the collection (contributed
  by Endefx)
- Updated translations

### 2022-12-01

- Updated to Hearthstone Version 25.0.0.159202 (contributed by Endefx)

### 2022-11-30

- Added the Death Knight corpse counter (contributed by Endefx)
- Updated to Hearthstone version 25.0.0.158725 (contributed by Endefx)

[06] Contributing to development
--------------------------------

Development of Hearthstone Access is based on a development tools repository
Guide Dev made available after he finished maintaining Hearthstone Access:  
<https://github.com/HearthstoneAccess/DevTools>  
The work for the community version is currently done in a fork of that
repository:  
<https://github.com/antonshusharin/DevTools>  
Best place to discuss the development of Hearthstone Access is the
ask-the-developers channel on the Hearthstone Access discord:
<https://discord.gg/WZWRenbuRe>