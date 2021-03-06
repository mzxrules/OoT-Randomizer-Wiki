# Setting Information

The OoT Randomizer offers many different settings to customize your play experience. Here's a fully detailed list!

# ROM Options

## Base Rom

Specify the input ROM that will be used by the randomizer. Please be sure it is OoT US v1.0.

## Output Directory

Specify where the output ROM will be written on your computer.

## Create Spoiler Log

Decide whether to output a text file detailing where every item can be found and the sequence of play that will lead to seed completion. Selecting this option will
create a different item configuration than using otherwise identical settings without printing a log; this is intended to prevent cheating in race environments.

## Compress Rom

Decide the format of the output ROM. Compressed is generally recommended for most users; this is necessary for injection into a .wad for use on the Virtual Console,
and all known N64 emulators have significant crashing problems with uncompressed ROMs. Real N64 hardware doesn't care so generation time can be improved by using
the uncompressed option if you are playing on a real N64 with a flash cart. You can also choose not to output a ROM at all; this is useful if you just want to look
at spoiler logs.

## Default Targeting Option

This option specifies whether Z-targeting will default to "Switch" or "Hold" style. Either way, this can still be changed in-game as per usual.

## Multi-World Generation

This option allows for multiple worlds to be generated to be used in co-op play. Each player will get a different ROM designed to work in conjunction with another
to allow two players to work together to complete the game. Synchronization can be achieved on Bizhawk via the following script:

https://github.com/TestRunnerSRL/bizhawk-co-op

### Player Count

Use this to specify how many players will be participating in this co-op playthrough.

### Player ID

Use this to specify which player number you are in particular. Each participant in the co-op should choose a different number starting with 1.

## Setting String

This is an 18 character string that specifies the totality of other gameplay relevant (non-cosmetic) settings used throughout the randomizer. This string can be shared
between players and then the "Import Settings String" button can be pressed to automatically change all settings to match another player.

## Seed

This is a string representing the particular configuration of items that will occur in your seed; the purpose is to combine a seed string with an identical settings
string such that the randomizer will be able to generate the same game for multiple players. If this field is left blank, a random seed will be chosen.

# Main Rules

## Open Forest

Mido does not need to see a sword and shield to reach the Deku Tree and the Kokiri boy blocking the exit to the forest is gone. If this flag is not set, it is
guaranteed that the Deku Tree can be completed without leaving the forest. This means that within the forest or the Deku Tree itself it will be possible to find
the Kokiri Sword, Deku Shield for sale, and the Slingshot.

## Open Kakariko Gate

The gate leading up Death Mountain from Kakariko Village is open from the beginning of the game. Normally this requires Zelda's Letter to open. This allows more
diverse routing early in the game and prevents very long walks in seeds with the Weird Egg shuffled. Two things are important to note. Showing Zelda's Letter to
the guard is still required to begin the Happy Mask sidequest and to receive a discount on purchasing Hylian Shields. The gate is simply gone for an adult no
matter what.

## Open Door of Time

The Door of Time is open from the beginning of the game. The Song of Time is still potentially useful to move Song of Time blocks, play songs for the frogs on Zora
River, or for other such uses. If this flag is not used, the Door of Time must be opened to become an adult as in the original game, but all that is needed to open
the Door of Time is the Song of Time and any ocarina. The Ocarina of Time in particular and the Spiritual Stones have nothing to do with this.

## Gerudo Fortress

### Default Behavior

Gerudo Fortress will work the same way it did in the original game. All four carpenters must be rescued in order for the Gerudo woman who gives the Gerudo Card to
appear and for the Gerudo to stop being hostile. Rescuing a carpenter requires having a Gerudo Fortress Small Key and defeating the corresponding guard.

### Rescue One Carpenter

Only the bottom left carpenter must be rescued to complete Gerudo Fortress. Only one Gerudo Fortress Small Key will exist because of this.

### Start with Gerudo Card

The player will start with the Gerudo Card from the beginning of the game. The carpenters will be pre-rescued, and the bridge to Gerudo Fortress as an adult will
be repaired from the beginning. The Gerudo Card is the requirement in the randomizer to enter Gerudo Training Grounds so it will be an accessible area from the
moment adulthood is available.

## Rainbow Bridge Requirement

This determines the condition under which the rainbow bridge to Ganon's Castle will spawn.

### All Dungeons

The rainbow bridge spawn requires all medallions and spiritual stones to be in the player's possession.

### All Medallions

All six of the medallions are required to open Ganon's Castle.

### Vanilla

The rainbow bridge spawns under the same conditions it did in the original game, possession of the Light Arrows and having viewed the Zelda cutscene. This
cutscene in the Temple of Time is triggered by possessing the Shadow and Spirit Medallions.

### Open

The rainbow bridge is always present.

## Random Number of Ganon's Trials

A random number of trials within Ganon's Castle from 0 to 6 will be chosen, and individual trials will be randomly disabled as necessary to match this number.
Alternatively, a specific number of trials can be specified with the slider below. If a number of trials other than 0 or 6 is chosen and hints are enabled,
hints will be added to the hint pool informing the player which trials are present (if 1 to 3 trials) or which are missing (if 4 or 5 trials).

## All Locations Reachable

This option will set the logic to try to ensure Link can reach every item location in the game with the exception of "key for key" item locations (a single
item spot behind a locked door containing the key to open the door). If this option is not used, the logic will allow some items to be in impossible locations
so long as the set of reachable items is sufficient to complete the game.

## Bombchus Are Considered in Logic

This option fundamentally changes how the Bombchu items found around the world function. With this option on, Bombchus are a progression item and operate as
a form of progressive item. The first Bombchu pack found will be worth 20 Bombchus and subsequent packs will be worth 10 or 5 Bombchus. Finding Bombchus will
be considered as logical progression, and having found any Bombchus will be the condition to play Bombchu Bowling or buy Bombchu refills from shops. This flag
will also add Bombchu (5) buyable items to the shops in Kokiri Forest, Castle Town Bazaar, and Kakariko Bazaar. With this option off, randomly found Bombchu
items are not considered as logical progression, randomly found Bombchus will have specific denominations based on the values from the original game, and
finding a Bomb Bag is what enables playing Bombchu Bowling and buying Bombchus from shops which will not have their inventories edited.

## Dungeons Have One Major Item

This option places one "major item" and one only in each of the dungeons. For the purpose of the randomizer, the dungeons are defined as the eight dungeons that
contain either Medallions or Spiritual Stones as well as Bottom of the Well, Ice Cavern, Gerudo Training Grounds, and Ganon's Castle. The major items are any
item usable with a c-button that is not simply a form of ammo (Bombchus are major only if "Bombchus are considered in logic" is on), songs, Mirror Shield, swords,
tunics, boots, Double Defense, Magic Meter/Double Magic, Bullet Bags, Quivers, Bomb Bags, Strength Upgrades, Scales, Wallets, and the Stone of Agony. To be
clear, this means that rupees, ammo, Deku Stick and Deku Nut ammo expansions, Pieces of Heart, Heart Containers, Gold Skulltula Tokens, Maps, Compasses,
Small Keys, Boss Keys, Deku Shields, Hylian Shields, and Ice Traps are not considered major items. However, Small Keys and Boss Keys are considered major
items if the appropriate "keysanity" settings are used. Note that unlike with the distribution of dungeon specific items like keys, this flag does consider
the hands of the Desert Colossus as Spirit Temple locations, and to mirror the original game, Spirit Temple will get two items instead of just one.

## Master Quest Dungeons

With this option you can select a number of Master Quest dungeons to be included in your game. A value of 0 leaves all dungeons in their vanilla form. A value of 12 swaps each for its Master Quest form. 6 is an even mix of both. You may also opt for a random number of dungeons.

## Shuffle Kokiri Sword

This flag adds the Kokiri Sword to the shuffle. With it off, the Kokiri Sword will always be found in its original chest in the Kokiri Forest.

## Shuffle Weird Egg

This flag adds the Weird Egg given by child Malon to the shuffle. With this flag on, child Malon will give a random item and the Weird Egg must be located
to do the events at Hyrule Castle with Zelda and Impa. These events block interacting with Talon and Malon at Lon Lon Ranch as a child as well as Saria in
Sacred Forest Meadow and the Happy Mask sidequest.

## Shuffle Ocarinas

This flag adds both the Fairy Ocarina and the Ocarina of Time to the shuffle. The ocarinas are a progressive item; the first found will always be the Fairy
Ocarina with the second being the Ocarina of Time even though the two are functionally identical. Without this flag on, leaving the Kokiri Forest to the
Lost Woods bridge as a child will always grant one Ocarina and the other is always available at the gate of Castle Town as a child when all three Spiritual
Stones are in the player's possession.

## Shuffle Songs with Items

This flag adds the 12 standard ocarina songs to the shuffle as normal items. With this flag on, the spots that contained songs in the original game will
simply give Link a random item, and the songs can be found as items freely. Without this flag on, songs are still randomized but only between each other.
In either case, the Scarecrow's Song is not affected; it is still obtained by interacting with Bonooru at Lake Hylia first as a kid and then as an adult.

## Shuffle Gerudo Card

This flag shuffles the Gerudo Card into the general item pool. In the randomizer, this is required to gain access to Gerudo Training Grounds, but it does
not have any impact on the hostility of the Gerudo in Gerudo Fortress who still check for the carpenter rescue events. Without this flag, the Gerudo
Card is always given by the Gerudo woman who spawns after the final carpenter is rescued. If Gerudo Fortress is cleared from the beginning of the game,
the player starts the game with the Gerudo Card and this setting is voided.

## Shuffle Deku Salescrubs

This flag makes every Deku Scrub Salesman in the world sell a random item instead of only the three that sold permanent upgrades in the original game.
Using this flag adds the various low tier items the other scrubs sold to the item pool for the most part; the potion refills are replaced with Recovery
Hearts for Red Potions and blue rupees for Green Potions. For each Deku Scrub that sold arrows/seeds depending on age, there will be a 75% chance of
adding a 30 arrow item and a 25% chance of adding a 30 seed item to the pool. If this is set, once a Deku Scrub Salesman is used, it will disappear
from the world forever. The individual settings in the dropdown can be used to set the price of each Deku Scrub Salesman to 10 rupees, leave the prices
as what they were in the original game, or set each price to a random value from 0 to 99 rupees. In all cases, the text for the Deku Scrub Salesmen
will not update.

## Shopsanity

This setting randomizes the items sold in shops. When it is used, all shop items are randomly re-arranged among all 8 of the original game's shops.
This setting causes the Bombchu Shop to be open from the very beginning of the game, and this setting considers the two shops in adult Kakariko
Village to be distinct shops from the two similar shops in child Castle Town; however, the shops in Kokiri Forest, Goron City, and Zora Domain are
the same shops as both ages. This setting overrides the "Bombchus considered in logic" editing of the shop item pool.

### Off

This disables the Shopsanity feature.

### Shuffled Shops (0 Items)

This causes all of the Shopsanity features described above.

### Shuffled Shops (1-4 Items)

This not only causes all of the Shopsanity features described above, but it also adds 1-4 (depending on the exact setting) items from the general
item pool into shops to buy for randomly chosen amounts of money. Lower value shop items are removed to make room for this, and low value junk items
are added to the item pool to fill the extra empty chests this will implicitly create. Using this feature will also replace several of the rupee
items found throughout the seed with higher value rupees and will add a third Wallet upgrade, the "Tycoon's Wallet", to the item pool which can hold
up to 999 rupees. The items from the general item pool added to shops will always be on the far left of the shop inventories, and these items can
always be bought if the player has enough rupees even if they are explosives without an appropriate container or a tunic as a child.

### Shuffled Shops (Random Items)

This is similar to the 1-4 items variant but gives each shop a random number of new items from 0-4. Each shop can have a different amount of unique
items with this setting.

## Shuffle Dungeon Items

This setting allows the player to decide the natural distribution of dungeon items. Dungeon items can be found confined to their original dungeons,
spread freely throughout the world, or prevented from existing completely. Items that are prevented from existing completely will be replaced in the
item pool with an assortment of various low tier junk items. This feature can be specified for Maps/Compasses, Small Keys, and Boss Keys independently.
If Small Keys or Boss Keys are prevented from existing, this will also remove all locks those keys would be used for from existing as well. If Small Keys
are left in their original dungeons and the Fire Temple is not in the form of Master Quest, the locked door in the first room that leads to the normal
location of the Boss Key will be removed.

## Maps and Compasses Give Information

This setting, only available if you start with Maps and Compasses or they are spread across the world, disables the pedestal in the Temple of Time from giving information about
the location of the Medallions and Spiritual Stones. Instead, the Compass from each of the eight eligible dungeons will tell the player which dungeon has
which reward. If Master Quest dungeons are to be mixed in, each of the ten Maps will tell the player whether any given dungeon is in the vanilla or Master Quest
form. The Compasses from Bottom of the Well and Ice Cavern do not give any information.

## Remove Ganon's Door Boss Lock

This setting removes the Boss Key lock from Ganon's Tower. This removes the need to locate the Ganon's Tower Boss Key to finish the game.

## Tokensanity

This setting shuffles the Gold Skulltula item drops into the general pool of locations. The player can choose only to include Gold skulltulas
found in dungeons for a more mild version of this setting.

# Detailed Logic

## Maximum Expected Skulltula Tokens

This setting can be used to reduce the number of Gold Skulltula Tokens that may be required to finish the game.

## No Nighttime Skulltulas without Sun's Song

This setting causes the logic to expect the player to have an ocarina and the Sun's Song to get Gold Skulltula locations that are only found at
nighttime.

## No Big Poes

This setting will guarantee that the Big Poe vendor will not have an important item.

## No Child Fishing

This setting will guarantee that the reward from child fishing is not an important item. This is mostly recommended if the player simply must play
on Bizhawk.

## No Adult Fishing

This setting will guarantee that the reward from adult fishing is not an important item. This is mostly recommended if the player simply must play
on Bizhawk.

## No Skull Mask Reward

This setting will guarantee that the item obtained from showing the Skull Mask in the Deku Theater is not an important item.

## No Mask of Truth Reward

This setting will guarantee that the item obtained from showing the Mask of Truth in the Deku Theater is not an important item.

## No 1500 Horseback Archery

This setting will guarantee that the item obtained from scoring 1500 points at the horseback archery challenge at Gerudo Fortress is not an
important item.

## No Lost Woods Memory Game

This setting will guarantee that the item obtained from winning the ocarina memory game in the Lost Woods is not an important item.

## No Racing Dampe a Second Time

This setting will guarantee that the item obtained from finishing with a sub-minute time in the second Dampe race is not an important item.

## No Biggoron Reward

This setting will guarantee that the item obtained from showing the Claim Check to Biggoron is not an important item.

## Adult Trade Sequence

This pair of settings can be used to specify the earliest and latest items that can be allowed to randomly show up in the general item pool.
Only one item will be in the item pool regardless of this setting; this can merely be used to limit the range of possibilities.

## Enable All Tricks

This is a button to turn on all of the trick related flags.

## Various Advanced Tricks

This setting allows a huge number of minor tricks to be allowed by the logic. Here is a complete list:

-A precise jumpslash with either a Deku Stick or the Kokiri Sword can be used to reach a Gold Skulltula on some vines in standad Deku Tree.
-The Bow can be used to knock down the stairs in Dodongo's Cavern with two well timed shots.
-The vines in Forest Temple leading to where the well drain switch is in the standard form can be barely reached with the standard Hookshot.
-The well in Forest Temple can be crossed with just Hookshot by shooting as low as possible on the vines from the far side and swimming under
the ceiling. This is possible in both versions but can only be required in Forest Temple MQ.
-A Bombchu from the ground level can be used to hit the switch to bypass the block pushing puzzle in Forest Temple MQ.
-A rusted switch under a Song of Time block in the standard Fire Temple can be hit by using Hammer into the block.
-The location with the Boss Key chest in Fire Temple MQ can be reached without the Bow with very particular use of Din's Fire.
-The upper levels of the old boulder maze in Fire Temple MQ can be reached without explosives by using the Hammer through a wall.
-In the standard Spirit Temple, the bridge on child side can be lowered with a carefully timed Bombchu.
-The frozen switch in Spirit Temple MQ can be hit without a fire source by using the Bow and Song of Time very cleverly.
-The chest in the basement of the standard Bottom of the Well can be reached with only a Strength Upgrade by using a jump slash with a lit
Deku Stick to access the bomb flowers in the basement.
-The silver rupees on the left side of Gerudo Training Grounds MQ can be collected with just Hookshot with a somewhat particular jump slash.
-The first room of the Spirit Trail in Ganon's Castle MQ can be cleared without the Bow by using a Hammer jump slash to hit the rusted switch
through the thrones.
-The Gold Skulltula in adult Kokiri Forest can be reached without the Hookshot by using Hover Boots off one of the roots.
-The child can reach the chest on Death Mountain trail with just the Goron Bracelet by backwalking with the Bomb Flower intended to open
Dodongo's Cavern and throwing the Bomb Flower at the wall very quickly.
-Gerudo Fortress can be cleared without any items other than those needed for access. The logic normally guarantees one of the Bow, Hookshot, or
Hover Boots to help navigate the "kitchen".

Using this setting will also pre-set all of the lower logic flags to a reasonable configuration to match the trick level. These can then be
edited as the player desires if the given configuration isn't desired.

## Man on Roof without Hookshot

This allows the logic to consider a trick in which the player does a sidehop off the tall tower in Kakariko Village to reach the man on the
rooftop with no items.

## Child Deadhand without Kokiri Sword

This allows the logic to consider defeating the Deadhand in Bottom of the Well with Deku Sticks. This is not hard with use of the power crouch
stab glitch, but consistently landing actual jump slashes on his unusual hitbox is pretty difficult and using normal slashes consumes 9 Deku Sticks.

## Dodongo's Cavern Spike Trap Room Jump without Hover Boots

This allows the logic to consider that the adult can make a particularly useful jump in Dodongo's Cavern to reach the area with the Bomb Bag chest early.
Due to the precision of the jump, normally the logic expects Hover Boots to complete this path.

## Windmill PoH as Adult with Nothing

This allows the logic to consider a jump the adult can make in the windmill to reach the Piece of Heart within with no items. The jump requires leaping
from an object on which it is not obvious Link is allowed to stand and has counterintuitive timing so it is not in standard logic.

## Crater's Bean PoH with Hover Boots

This allows the logic to consider using Hover Boots to reach the Piece of Heart atop the volcano in Death Mountain Crater. The path involves walking up a
very steep slope that is not visibly walkable so it is not in normal logic.

## Zora's Domain Entry with Cucco

This allows the logic to consider using a Cucco on Zora River to enter Zora's Domain as a child without playing Zelda's Lullaby. It requires slipping behind
the waterfall trickily from the left side.

## Zora's Domain Entry with Hover Boots

This allows the logic to consider this similar trick to the above except as an adult with Hover Boots. This is actually a lot more difficult even though it can
be done from either side of the waterfall.

## Fewer Tunic Requirements

This relaxes the tunic requirements by the logic somewhat. Normally the logic expects a Goron Tunic to enter Fire Temple or complete the Fire Trial in Ganon's Castle
and a Zora Tunic to enter Water Temple, collect the underwater silver rupees in Gerudo Training Grounds, or obtain the Piece of Heart at the bottom of the frozen Zora's
Fountain. With this flag set, the Goron Tunic will not be required to actually enter Fire Temple, only to fight Volvagia or to reach the upper floors. The Zora Tunic
requirements are removed completely except to reach the chest at the bottom of the central pillar in Water Temple.

## Morpha with Gold Scale

This setting allows entry to the Water Temple with the Gold Scale to be considered. Since you cannot backtrack into Water Temple without Iron Boots, only the Spiritual
Stone or Medallion obtained from defeating Morpha can be considered by logic either way; since you need the Water Temple Boss Key and Longshot to access Morpha normally,
this means that this setting is only relevant in either keysanity or keysy relative to the locations of Boss Keys.

## Lens of Truth

This setting alters the expectations about interacting with invisible objects without the Lens of Truth.

### Required Everywhere

This setting requires the Lens of Truth to interact with any invisible object except for whatever was required in the original game to obtain the Lens of Truth.

### Wasteland and Chest Minigame

This setting expects the Lens of Truth to be used only to cross the Haunted Wasteland and to win the Treasure Chest Minigame in Castle Town at night.

### Only Chest Minigame

This setting expects the Lens of Truth to be used only to win the Treasure Chest Minigame in Castle Town at night.

# Other

## Skip Tower Collapse Sequence

This setting causes defeating Ganondorf to skip directly to the Ganon fight without the need to do the collapsing Ganon's Tower sequence.

## Skip Interior Castle Guard Stealth Sequence

This setting causes entering the crawlspace at Hyrule Castle to deposit the player directly into the Castle Courtyard, bypassing the guard
evasion sequence.

## Skip Epona Race

This setting causes Epona to be stolen from Ingo from the start of the game, only requiring Epona's Song and an ocarina as an adult to summon.

## Fast Chest Cutscenes

This setting causes all chests to open with a quick animation. If this setting is off, certain important items will trigger the slow opening animation.

## Random Big Poe Target Count

This setting causes the number of Big Poes that must be turned into the vendor to obtain his item to be random from 1-10. Alternatively, the number
of Big Poes requires can be selected manually with the slider below. Note that Big Poes can be found as pre-stocked Bottle contents, and the logic
can expect using them if the required number is sufficiently low.

## Start with Scarecrow's Song

This flag causes Pierre the Scarecrow to be available to summon for the adult from the beginning of the game. The box below can be used to
specify the particular desired Scarecrow's Song. This song must be exactly eight notes long and must contain at least two different notes.

## Randomize Ocarina Song Notes

This flag randomizes the particular notes in the 12 standard ocarina songs. This can predictably be pretty obnoxious. In general, the patterns chosen
for the top row songs will be simpler than the patterns chosen for warp songs.

## Chest Size Matches Contents

This flag causes keys, Ice Traps, and items flagged as progression items to appear in large treasure chests while other items will be in small treasure chests.
This means that players can choose to skip small treasure chests since they will only contain handy, not essential, items.

## Clearer Hints

This flag changes the text of Gossip Stone hints to be overwhelmingly explicit. This is helpful for players who do not have English as their first language,
but the hints will be less "fun" and less like the sorts of things that would be said in the original game.

## Gossip Stones

This flag changes the behavior of Gossip Stones to give hints to players. The hints will be distributed as such:

-If the required number of trials is 1-3, a hint will be added for each trial that must be done. If the required number of trials is 4 or 5, a hint will be added
for each trial that can be skipped.
-Hints will be added for every one of the "always" locations that is allowed to have a random possibly valuable item under the current settings. These hints
will tell the player what item is at each of these locations. These locations are the rewards for 30, 40, and 50 Gold Skulltula Tokens, the item obtained from
Biggoron by showing the Claim Check, the item obtained from the Big Poe vendor, both the song and the item slots at the Ocarina of Time, and the item obtained
from showing the Mask of Truth at the Deku Theater.
-Some hints will be given for items at a randomly selected number of other locations that are generally somewhat inconvenient to check. The total number of these
hints will be either 11 or 12 minus the number of always hints placed.
-3 or 4 hints will be given naming a specific non-dungeon specific item that can be found in a randomly chosen dungeon.
-1 to 4 hints will be given naming a specific item found in a specific overworld region. Which part of this range is used is determined in part by how many
trial hints are given.
-4 to 6 hints will be given naming what region specific progression items other than Gold Skulltula Tokens can be found.
-3 or 4 hints will be given naming specific regions that are "on the way of the hero" and thus contain at least one required progression item.
-All remaining hints (33 total unique Gossip Stones exist) will be filled with non-information junk hints.

This setting allows the player to specify which item is required to interact with the Gossip Stones. The Stone of Agony is the default option as it gives a
fairly purposeless vanilla item a use and allows both kid and adult to interact with the Gossip Stones. The default Mask of Truth can be used, but this has
the downside that the Mask of Truth can only be obtained with all Spiritual Stones which tends to make the hints not useful, and using the Mask of Truth
requires being a child which is another big downside. There is also an option for the information to just be free for those wanting an easier mode.

## Text Shuffle

This setting allows all the text in the game to be shuffled. This is mostly for comedy and is not intended to be a serious gameplay option.

### No Text Shuffled

Leave the text alone.

### Shuffled except Hints and Keys

Shuffle all text other than the useful text giving the player information.

### All Text Shuffled

Shuffle all text even to the player's mechanical disadvantage.

## Difficulty

This setting allows the player to tweak the item pool to make a somewhat harder experience.

### Normal

Leave the item pool alone.

### Hard

Heart Containers, Double Defense, and the second Magic Upgrade are replaced with junk items. One each
of the ammo expansions (Quiver, Bullet Bag, Bomb Bag Deku Stick Capacity, Deku Nut Capacity) will also
be replaced with junk items, and all Bombchu pick-ups other than three will similarly be replaced with
junk.

### Very Hard

In addition to the items from Hard, Pieces of Heart and Nayru's Love are also replaced with junk items.
One more of each ammo expansion is removed resulting in zero extra ammo capacity for those item types,
and only one Bombchu pick-up can be found.

## Damage Multiplier

This setting changes the amount of damage taken.

### Normal

Link takes normal damage.

### OHKO

Link dies in one hit. Ice Traps are removed, and at least one Nayru's Love is in the item pool.

# Cosmetics

## Background Music

### Normal

Do not alter the background music.

### No Music

Disable background music. Sound effects will still play. This may be desired by players who like to listen to their own music.

### Random

Background music is shuffled so that different tracks may play in different areas. This may be silly.

## Kokiri Tunic Color

This determines the color of Link's default Kokiri Tunic. This only affects the color when he's wearing it, not the color of the icon in the menu.

### Most Colors

Simply get the particular color selected. Available colors are Kokiri Green, Goron Red, Zora Blue, Black, White, Azure Blue, Vivid Cyan, Light Red,
Fuchsia, Purple, MM Purple, Twitch Purple, Purple Heart, Persian Rose, Dirty Yellow, Blush Pink, Hot Pink, Rose Pink, Orange, Gray, Gold, Silver,
Beige, Teal, Blood Red, Blood Orange, Royal Blue, Sonic Blue, NES Green, Dark Green, and Lumen.

### Random Choice

Choose a random color from the set of pre-made colors.

### Completely Random

Generate a random color with numerically random RGB values.

### Custom Color

A special interface will pop up that will allow the user to choose any color from a diverse color wheel or input a desired RGB value.

## Goron Tunic Color

This determines the color of Link's Goron Tunic. This only affects the color when he's wearing it, not the color of the icon in the menu or when
holding it up after acquiring it. The options are identical to those for the Kokiri Tunic.

## Zora Tunic Color

This determines the color of Link's Zora Tunic. This only affects the color when he's wearing it, not the color of the icon in the menu or when
holding it up after acquiring it. The options are identical to those for the Kokiri Tunic.

## Low Health SFX

This determines which sound effect to play repeatedly when Link is very low on health. Several of these options are designed to be potentially
more pleasant to listen to while a few are designed to be more amusing.

### Particular Sounds

Set this particular sound for the heart beep. Available choices are Default, Softer Beep, Rupee, Timer, Tambourine, Recovery Heart, Carrot Refill,
Navi - Hey!, Zelda - Gasp, Cluck, Mweep!, Iron Boots, Hammer, Sword Bounce, Bow, Gallop, Drawbridge, Switch, Bomb Bounce, Bark, Ribbit, Broken Pot,
Business Scrub, Guay, and Bongo Bongo. Indeed, one of these is the sound a king might make when moving... very slowly.

### Random Choice

Play a random SFX from the list of choices.

### None

Disable low health heart beeps altogether.

## Navi Color

These options can be used to set Navi's color in a variety of contexts. The lists of pre-set colors here is different, but the same types of options
exist as for choosing tunic colors.

## Navi Hint

This option sets the SFX that will play when Navi is ready to give a hint. The options are very similar to the Low Health SFX.

## Navi Enemy Target

This option sets the SFX that will play when Navi targets an enemy. The options are very similar to the Low Health SFX.

# Command Line Options

```
-h, --help
```

Show the help message and exit.

```
--check_version
```

Check for the latest version number online (default: False)

```
--checked_version CHECKED_VERSION
```

Check for the specified version number instead of a number from online.

```
--rom ROM
```

Path to a The Legend of Zelda: Ocarina of Time NTSC-US v1.0 ROM. (default: ZOOTDEC.z64)

```
--output_dir OUTPUT_DIR
```

Path to output directory for rom generation.

```
--seed SEED
```

Define seed number to generate. (default: None)

```
--count COUNT
```

Set the count option (default: None)

```
--world_count WORLD_COUNT
```

Use to create a multi-world generation for co-op seeds. World count is the number of players.
Warning: Increasing the world count will drastically increase generation time. (default: 1)

```
--player_num PLAYER_NUM
```

Use to select world to generate when there are multiple worlds. (default: 1)

```
--create_spoiler
```

Output a Spoiler File (default: False)

```
--compress_rom [{True,False,None}]
```

Create a compressed version of the output rom file.
True: Compresses. Improves stability. Will take longer to generate
False: Uncompressed. Unstable on emulator. Faster generation
None: No ROM Output. Creates spoiler log only (default: True)

```
--open_forest
```

Set whether Kokiri children obstruct your path at the beginning of the game. (default: False)

```
--open_kakariko
```

The gate in Kakariko Village to Death Mountain Trail is always open, instead of needing Zelda's Letter. (default: False)

```
--open_door_of_time
```

Set whether the Door of Time is open from the beginning of the game. (default: False)

```
--gerudo_fortress [{normal,fast,open}]
```

Select how much of Gerudo Fortress is required. (default: normal)

```
--bridge [{medallions,vanilla,dungeons,open}]
```

Select the condition to spawn the Rainbow Bridge to Ganon's Castle. (default: medallions)

```
--all_reachable
```

Enables the "Only Ensure Seed Beatable" option (default: False)

```
--all_reachable
```

Enables the "Only Ensure Seed Beatable" option (default: False)

```
--bombchus_in_logic
```

Changes how the logic considers Bombchus and other Bombchu related mechanics (default: False)

```
--one_item_per_dungeon
```

Each dungeon will have exactly one major item. (default: False)

```
--trials_random
```

Sets the number of trials that must be cleared in Ganon's Castle to a random value (default: False)

```
--trials [{0,1,2,3,4,5,6}]
```

Sets the number of trials that must be cleared in Ganon's Castle (default: 6)

```
--no_escape_sequence
```

Removes the tower collapse sequence after defeating Ganondorf (default: False)

```
--no_guard_stealth
```

Removes the guard evasion sequence in Hyrule Castle (default: False)

```
--no_epona_race
```

Removes the need to race Ingo to acquire Epona (default: False)

```
--fast_chests
```

Causes all chests to open with a fast animation (default: False)

```
--big_poe_count_random
```

Sets the number of Big Poes that must be sold to the vendor for an item to a random value (default: False)

```
--big_poe_count [{1,2,3,4,5,6,7,8,9,10}]
```

Sets the number of Big Poes that must be sold to the vendor for an item (default: 10)

```
--free_scarecrow
```

Start the game with the Scarecrow's Song activated and Pierre possible for the adult to summon (default: False)

```
--scarecrow_song [SCARECROW_SONG]
```

Set Scarecrow's Song if --free_scarecrow is used. Valid notes: A, U, L, R, D (default: DAAAAAAA)

```
--shuffle_kokiri_sword
```

Include the Kokiri Sword as a randomized item (default: False)

```
--shuffle_weird_egg
```

Include the Weird Egg as a randomized item (default: False)

```
--shuffle_ocarinas
```

Include the two ocarinas as randomized items (default: False)

```
--shuffle_song_items
```

Treat the ocarina songs as normal items and shuffle them into the general item pool (default: False)

```
--shuffle_gerudo_card
```

Include the Gerudo Card to access Gerudo Training Grounds as a randomized item (default: False)

```
--shuffle_scrubs [{off,low,regular,random}]
```

Include all Deku Scrub Salesmen as randomized item and determine their prices (default: off)

```
--shopsanity [{off,0,1,2,3,4,random}]
```

Randomize shop items and add the chosen number of items from the general item pool to shop inventories (default: off)

```
--shuffle_mapcompass [{remove,startwith,dungeon,keysanity}]
```

Choose the locations Maps and Compasses can be found (default: dungeon)

```
--shuffle_smallkeys [{remove,dungeon,keysanity}]
```

Choose the locations Small Keys can be found (default: dungeon)

```
--shuffle_bosskeys [{remove,dungeon,keysanity}]
```

Choose the locations Boss Keys can be found (default: dungeon)

```
--enhance_map_compass
```

Change the functionality of the Map and Compass to give information about their dungeons. The Temple of Time Altar will no longer provide any dungeon information. (default: False)

```
--unlocked_ganondorf
```

Remove the Boss Key door leading to Ganondorf (default: False)

```
--tokensanity [{off,dungeons,all}]
```

Include the chosen Gold Skulltula Token locations in the item shuffle (default: off)

```
--mq_dungeons_random
```

Sets the number of Master Quest dungeons to a random value (default: False)

```
--mq_dungeons [{0,1,2,3,4,5,6,7,8,9,10,11,12}]
```

Sets the number of Master Quest dungeons (default: 0)


```
--logic_skulltulas [{0,10,20,30,40,50}]
```

Choose the maximum number of Gold Skulltula Tokens that could be required (default: 50)

```
--logic_no_night_tokens_without_suns_song
```

Change logic to expect Sun's Song to defeat nighttime Gold Skulltulas (default: False)

```
--logic_no_big_poes
```

Prevent the Big Poe vendor from having a required item (default: False)

```
--logic_no_child_fishing
```

Prevent the prize from fishing as a child from being a required item (default: False)

```
--logic_no_adult_fishing
```

Prevent the prize from fishing as an adult from being a required item (default: False)

```
--logic_no_trade_skull_mask
```

Prevent the item obtained by showing the Skull Mask at the Deku Theater from being a required item (default: False)

```
--logic_no_trade_mask_of_truth
```

Prevent the item obtained by showing the Mask of Truth at the Deku Theater from being a required item (default: False)

```
--logic_no_1500_archery
```

Prevent the item obtained by scoring 1500 points at horseback archery from being a required item (default: False)

```
--logic_no_memory_game
```

Prevent the item obtained by completing the ocarina memory game in the Lost Woods from being a required item (default: False)

```
--logic_no_second_dampe_race
```

Prevent the prize won by finishing the second Dampe race in under 1 minute from being a required item (default: False)

```
--logic_no_trade_biggoron
```

Prevent the item obtained by showing the Claim Check to Biggoron from being a required item (default: False)

```
--logic_earliest_adult_trade [{pocket_egg,pocket_cucco,cojiro,odd_mushroom,poachers_saw,broken_sword,prescription,eyeball_frog,eyedrops,claim_check}]
```

Set the earliest item in the adult trade sequence that can be found in the item pool (default: pocket_egg)

```
--logic_latest_adult_trade [{pocket_egg,pocket_cucco,cojiro,odd_mushroom,poachers_saw,broken_sword,prescription,eyeball_frog,eyedrops,claim_check}]
```

Set the latest item in the adult trade sequence that can be found in the item pool (default: claim_check)

```
--logic_tricks
```

Enable the logic to consider a large number of minor tricks (default: False)

```
--logic_man_on_roof
```

Enable the logic to consider the trick to reach the man on the roof in Kakariko Village with a sidehop from the tower (default: False)

```
--logic_child_deadhand
```

Enable the logic to consider the child defeating Deadhand with only Deku Sticks (default: False)

```
--logic_dc_jump
```

Enable the logic to consider the trick to bypass the second Lizalfos fight room in Dodongo's Cavern as an adult with a simple jump (default: False)

```
--logic_windmill_poh
```

Enable the logic to consider the trick to reach the Piece of Heart in the windmill as an adult with nothing (default: False)

```
--logic_crater_bean_poh_with_hovers
```

Enable the logic to consider the trick to reach the Piece of Heart on the volcano in Death Mountain Crater with Hover Boots (default: False)

```
--logic_zora_with_cucco
```

Enable the logic to consider the trick to enter Zora's Domain as a child using a Cucco instead of playing Zelda's Lullaby (default: False)

```
--logic_zora_with_hovers
```

Enable the logic to consider the trick to enter Zora's Domain as an adult using Hover Boots instead of playing Zelda's Lullaby (default: False)

```
--logic_fewer_tunic_requirements
```

Reduce the number of locations for which the logic expects a tunic upgrade (default: False)

```
--logic_morpha_with_scale
```

Allows entering Water Temple and beating Morpha with Gold Scale instead of Iron Boots. The Longshot and Boss Key are still required to reach the boss.
This means that this option is only relevant in keysanity or keysy. (default: False)

```
--logic_lens [{chest,chest-wasteland,all}]
```

Set which hidden objects the logic expects the Lens of Truth to be used on (default: all)

```
--ocarina_songs
```

Randomize the particular notes that must be played for each of the 12 standard ocarina songs (default: False)

```
--correct_chest_sizes
```

Set chest sizes based on contents (default: False)

```
--clearer_hints
```

Reword hints to be incredibly direct (default: False)

```
--hints [{none,mask,agony,always}]
```

Enable hints from Gossip Stones and select the condition to read them (default: agony)

```
--text_shuffle [{none,except_hints,complete}]
```

Shuffle the chosen text randomly (default: none)

```
--difficulty [{normal,hard,very_hard}]
```

Alter the item pool to increase difficulty. (default: normal)

```
--damage_multiplier [{normal,ohko}]
```

Alters the amount of damage taken. The ohko option causes Link to die in one hit. (default: normal)

```
--default_targeting [{hold,switch}]
```

Set the default Z-targeting setting. It can still be changed in the game's options menu. (default: hold)

```
--background_music [{normal,off,random}]
```

Choose whether the game's background music will be left alone, disabled, or shuffled randomly. (default: normal)

```
--kokiricolor [{'Random Choice', 'Completely Random', 'Kokiri Green', 'Goron Red', 'Zora Blue', 'Black', 'White', 'Azure Blue', 'Vivid Cyan', 'Light Red', 'Fuchsia', 'Purple', 'MM Purple', 'Twitch Purple', 'Purple Heart', 'Persian Rose', 'Dirty Yellow', 'Blush Pink', 'Hot Pink', 'Rose Pink', 'Orange', 'Gray', 'Gold', 'Silver', 'Beige', 'Teal', 'Blood Red', 'Blood Orange', 'Royal Blue', 'Sonic Blue', 'NES Green', 'Dark Green', 'Lumen'}]
```

Select the color of Link's Kokiri Tunic. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Kokiri Green)

```
--goroncolor [{'Random Choice', 'Completely Random', 'Kokiri Green', 'Goron Red', 'Zora Blue', 'Black', 'White', 'Azure Blue', 'Vivid Cyan', 'Light Red', 'Fuchsia', 'Purple', 'MM Purple', 'Twitch Purple', 'Purple Heart', 'Persian Rose', 'Dirty Yellow', 'Blush Pink', 'Hot Pink', 'Rose Pink', 'Orange', 'Gray', 'Gold', 'Silver', 'Beige', 'Teal', 'Blood Red', 'Blood Orange', 'Royal Blue', 'Sonic Blue', 'NES Green', 'Dark Green', 'Lumen'}]
```

Select the color of Link's Goron Tunic. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Goron Red)

```
--zoracolor [{'Random Choice', 'Completely Random', 'Kokiri Green', 'Goron Red', 'Zora Blue', 'Black', 'White', 'Azure Blue', 'Vivid Cyan', 'Light Red', 'Fuchsia', 'Purple', 'MM Purple', 'Twitch Purple', 'Purple Heart', 'Persian Rose', 'Dirty Yellow', 'Blush Pink', 'Hot Pink', 'Rose Pink', 'Orange', 'Gray', 'Gold', 'Silver', 'Beige', 'Teal', 'Blood Red', 'Blood Orange', 'Royal Blue', 'Sonic Blue', 'NES Green', 'Dark Green', 'Lumen'}]
```

Select the color of Link's Zora Tunic. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Zora Blue)

```
--navicolordefault [{'Random Choice', 'Completely Random', 'Gold', 'White', 'Green', 'Light Blue', 'Yellow', 'Red', 'Magenta', 'Black', 'Tatl', 'Tael', 'Fi', 'Ciela', 'Epona', 'Ezlo', 'King of Red Lions', 'Linebeck', 'Loftwing', 'Midna', 'Phantom Zelda'}]
```

Select the color of Navi in idle. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: White)

```
--navicolorenemy [{'Random Choice', 'Completely Random', 'Gold', 'White', 'Green', 'Light Blue', 'Yellow', 'Red', 'Magenta', 'Black', 'Tatl', 'Tael', 'Fi', 'Ciela', 'Epona', 'Ezlo', 'King of Red Lions', 'Linebeck', 'Loftwing', 'Midna', 'Phantom Zelda'}]
```

Select the color of Navi when she is targeting an enemy. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Yellow)

```
--navicolornpc [{'Random Choice', 'Completely Random', 'Gold', 'White', 'Green', 'Light Blue', 'Yellow', 'Red', 'Magenta', 'Black', 'Tatl', 'Tael', 'Fi', 'Ciela', 'Epona', 'Ezlo', 'King of Red Lions', 'Linebeck', 'Loftwing', 'Midna', 'Phantom Zelda'}]
```

Select the color of Navi when she is targeting an NPC. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Light Blue)

```
--navicolorprop [{'Random Choice', 'Completely Random', 'Gold', 'White', 'Green', 'Light Blue', 'Yellow', 'Red', 'Magenta', 'Black', 'Tatl', 'Tael', 'Fi', 'Ciela', 'Epona', 'Ezlo', 'King of Red Lions', 'Linebeck', 'Loftwing', 'Midna', 'Phantom Zelda'}]
```

Select the color of Navi when she is targeting a prop. Can also set Custom (#RRGGBB) using hexadecimal RGB values to set a custom color. (default: Green)

```
--navisfxoverworld [{'Default', 'Random Choice', 'None', 'Cluck', 'Rupee', 'Softer Beep', 'Recovery Heart', 'Timer', 'Low Health', 'Notification', 'Tambourine', 'Carrot Refill', 'Zelda - Gasp', 'Mweep!', 'Ice Break', 'Explosion', 'Crate', 'Great Fairy', 'Moo', 'Bark', 'Ribbit', 'Broken Pot', 'Cockadoodledoo', 'Epona', 'Gold Skulltula', 'Redead', 'Poe', 'Ruto', 'Howl', 'Business Scrub', 'Guay', "H'lo!"}]
```

Select the sound effect that plays when Navi wishes to speak with the player. (default: Default)

```
--navisfxenemytarget [{'Default', 'Random Choice', 'None', 'Cluck', 'Rupee', 'Softer Beep', 'Recovery Heart', 'Timer', 'Low Health', 'Notification', 'Tambourine', 'Carrot Refill', 'Zelda - Gasp', 'Mweep!', 'Ice Break', 'Explosion', 'Crate', 'Great Fairy', 'Moo', 'Bark', 'Ribbit', 'Broken Pot', 'Cockadoodledoo', 'Epona', 'Gold Skulltula', 'Redead', 'Poe', 'Ruto', 'Howl', 'Business Scrub', 'Guay', "H'lo!"}]
```

Select the sound effect that plays when Navi targets an enemy. (default: Default)

```
--healthSFX [{'Default', 'Random Choice', 'None', 'Cluck', 'Softer Beep', 'Recovery Heart', 'Timer', 'Notification', 'Tambourine', 'Carrot Refill', 'Navi - Random', 'Navi - Hey!', 'Zelda - Gasp', 'Mweep!', 'Iron Boots', 'Hammer', 'Sword Bounce', 'Bow', 'Gallop', 'Drawbridge', 'Switch', 'Bomb Bounce', 'Bark', 'Ribbit', 'Broken Pot', 'Business Scrub', 'Guay', 'Bongo Bongo'}]
```

Select the sound effect that loops at low health. (default: Default)

```
--gui
```

Open the graphical user interface. Preloads selections with set command line parameters.

```
--loglevel [{error,info,warning,debug}]
```

Select level of logging for output. (default: info)

```
--settings_string SETTINGS_STRING
```

Enter a settings string that will encode and override most individual settings.
