# Changelog

## Unreleased

- Added the Demon Hunter Module
- Updates for 7.3.5 Legion patch compatability
- Fixed sound channels for new api
- Updated Classes for 8.0.0 Battle for Azeroth pre-patch

## Legacy Releases

### [v1.980.8] - 2012-09-27

- Rogue: Updated class module.
- Warrior: Updated class module.

### [v1.980.7]

- Monk: Added class module.
- Rogue: Updated class module. I'm still working on adding MoP spells.
- Spell Timer: Fixed bug related to spells that now have a self buff ánd a target debuff. I will investigate this problem further for the next update.

### [v1.980.6]

- Paladin: Updated class module.

### [v1.980.5]

- Druid: Updated class module.

### [v1.980.4]

- Hunter: Updated class module.
- Shaman: Updated class module.
- Warlock: Updated class module.
- General: Some fixes to the Options panel. You can now scroll all the way down again. Option tooltips are now loaded differently, so that you should never get a 'script ran too long' error.

### [v1.980.3]

- Mage: Updated class module.

### [v1.980.2]

- Priest: Updated class module.
- Warlock: Updated class module.

### [v1.980.1]

- Death Knight: Updated class module. Spells should now be more correct and complete.
- Warlock: Updated class module. Spells should now be more correct and complete.

### [v1.98]

- General: Works with Patch 5.0 / Mists of Pandaria.
- General: There are still lots of spells that need to be (re-)added, but at least it shouldn't give any lua errors. I will try to go through all classes in the coming weeks.
- General: The option to enable the display of registered spells to spell type groups is moved to 'Advanced Options > Options Behavior > List spells on mouse-over', because this now also applies to the Cooldown Timer.

### [v1.976.3]

- General: Added some internal/hidden cooldowns.
- Spell Timer: Fixed bug in de update of some Cooldowns on the Spell Timer, like Death Knight's Runes changing into Death Runes.
- Cooldown Timer: Internal/hidden cooldowns are now added to their own cooldown group, separate from Powerups.
- Cooldown Timer: You can now see what spells are hard-coded to the cooldown groups too (Advanced Options > Spell Timer > List spells on mouse-over).

### [v1.976.2]

- General: Hiding the tooltips on the Spell Timer works again.
- General: Removed old/dummy class modules from the addon package. You can safely delete all the class modules (Forte_DeathKnight, Forte_Druid, Forte_Hunter, Forte_Mage, Forte_Paladin, Forte_Priest, Forte_Rogue, Forte_Shaman, Forte_Vehicle, Forte_Warlock and Forte_Warrior). Make sure you keep and enable the Forte_Class module.
- General: Many spell ids across all modules have been corrected or removed.
- Spell Timer: You can see what spells belong to the spell type groups by mousing over their options. For real this time! ;) This is not enabled by default, so you have to go to 'Advanced Options > Spell Timer > List spells on mouse-over' to switch it on.
- Cooldown Timer: changed hidden cooldown of Lightweave to 65 seconds (from 45).

### [v1.976]/[v1.976.1]

- Spell Timer: Spells are now added to the class modules in a different way, which allows for much more flexibility. While this is super nice, I can't guarantee that everything still works as it should, simply because I can't test a lot myself.
- Spell Timer: Fixed many small bugs and features. E.g. all spells can now show their damage/healing ticks on the bars, not just damage-over-time spells.
- Spell Timer: You can now see Weapon enchants on the Spell Timer too.
- Spell Timer: You can see what spells belong to the spell type groups by mousing over their options.
- Spell Timer: Changed the spell types from their 'technical properties' to their practical use (e.g. crowd control type). I will further build on this in the next versions.
- Spell Timer: Mousing over Spell Timer icons will now also show the 'real' tooltip for the (de)buff or spell.
- Cooldown Timer: Ranged weapon enchants are now shown too.
- General: Mousing over a default button will now display the default in the option itself, instead of in the tooltip.
- General: Added a fix that allows '%' signs in Party/Raid messages, without giving errors. Before this fix only properly formatted text, like %% or %s was possible. This should at least fix the Recklessness message bug.
- General: The colour black (0.00 0.00 0.00) will now also work properly on 64-bit clients.
- IMPORTANT: All Class modules are now part of the Forte_Class Module. This will avoid problems because of class modules not being enabled. This will not impact the in-game performance. THE OLD CLASS MODULE FILES WILL REMAIN IN THE PACKAGE AS EMPTY DUMMIES FOR THE NEXT COUPLE OF UPDATES, TO AVOID MANUAL UPDATE PROBLEMS.

### [v1.975.9]

- Spell Timer: Fixed bug in channel timer updates. The duration would be wrong if you refreshed a channelled spell. When you get 'interrupted', the duration of channels is still more accurate than in the default WoW interface.
- Spell Timer: Fixed bug with timers without a real duration not being removed properly. 'Raid debuffs' were not affected by this bug.
- Warrior: Added a number of announcement messages to the Warrior class module. Thanks to KrazyKrl!
- General: Added a number of spells to various modules. This should be most of the requested spells from the last five months (that are possible at the moment).
- General: 'yell' is now also a valid output channel for the Party/Raid messages.
- General: I removed some compatibility fixes. Now you can no longer use the global frame names FX_Timer, FX_Cooldown and FX_Splash. Instead, just use the names FX_Timer1, FX_Cooldown1 and FX_Splash1.
- General: If you have problems with the font of the options interface in your language, you can use the command "/fx resetfont" to set it to a safe default.

### [v1.975.8]

- Version update to 4.3.0.
- Added some spells to the timer modules, but I will add more in the next update.

### [v1.975.7]

- Druid: Fixed the default message strings for Innervate and Rebirth in the Druid module.

### [v1.975.6]

- General: Added many small requested updates to spells! Feel free to tell me if I skipped anything.
- Cooldown Timer: Attempted to fix the spell grouping (mostly meant for Death Knights). Let me know if this causes any unwanted behaviour, because it certainly could...

### [v1.975.5]

- General: All modules should work with Patch 4.2. Don't install this update before 4.2 is live in your region!
- General: A few other small core and module fixes/updates.

**Note:** If DOTS keep turning red and falling off with this version on 4.2, switch off 'Advanced Options > Spell Timer > Improve : Use dot ticks'. I noticed on the PTR that damage ticks were not always properly showing up in the combat log, but this may be fine on Live servers.

### [v1.975.4]

- Spell Timer: fixed the Ghoul timer. It should again show up as a Pet bar, without you having to create a custom filter for it.
- Spell Timer: Added an accurate 'Army of the Dead' timer.
- Casting: Added a few new Druid party/raid messages. Thanks to Joseph Toth.
- Casting: Fixed bug in the cast whisper messages. They should now show up again.

### [v1.975.3]

- General: Frame positions now update when you change UI scale. You no longer need to reload or change options for them to get back in the right place. The Splash frame should now update its position properly too.
- Spell Timer: Added 'Archangel', 'Dark Archangel' and 'Evangelism' powerup buff for Priests.
- Spell Timer: Fixed 'Demoralizing Shout' duration when glyphed for Warriors.
- Spell Timer: Fixed bug in bar spacing when fading out. Would only be noticeable when you have a really high bar spacing and name tags/labels enabled though.
- Cooldown Timer: Cooldowns that are about to expire should no longer increase to the global cooldown time.
- Changed a bit of the config initialisation so people with a 'damaged' config no longer need to type '/fx usebackup' for FX to load properly. This is probably not needed any more, since most people will already have done this anyway, but you never know!

### [v1.975.2]

- If you still have problems after updating, type '/fx usebackup' and everything should work again.
- General: Fixed error in LUI version detection when an older LUI module was used.
- General: Updated the 'standard' time format to be able to display hours (h) too.

### [v1.975.1]

- General: Properly disabled all Talent Spy related code in the Core, so this will no longer give lua errors when you enter a party or raid.
- Spell Timer: Fixed localization error for non-English clients.

### [v1.975]

- When you run ### [v1.975, FX will keep a backup of your current settings and convert them for this new version. This means that you can revert back to a previous version, but if you do, your settings will also revert back!
- Options Interface: Cross-profile and Cross-clone linkable options. For information about how this works exactly, see this FAQ: [http://www.wowinterface.com/portal.php?id=513&a=faq&faqid=654]. You currently can't link the frame properties 'Lock, scale, alpha and position' yet (the options located in the option panel headers).
- Options Interface: You can see what options are not relevant for your current configuration. Note: The "All other..." spell types in the Spell and Cooldown timers are still permanently disabled; everything else can be enabled as intended by choosing a fitting configuration.
- Options Interface: The 'defaults' icons are also disabled when the option is currently set to its default. Defaults are now visible in the tooltip when you mouse over an active default button. I will probably change this in the future so mousing over will really show the defaults filled in their proper places, instead of showing them listed in the tooltip.
- Options Interface: You will only switch profile/clone if you deleted the currently selected one.
- Options Interface: Manually expanded/collapsed category states get saved. You can now also expand/collapse a whole options frame by clicking its header.
- General: The 'General Module Appearance' settings will now work for all Clones too.
- General: You can now change the font flags too.
- General: Fixed addon communication for patch 4.1.0.
- Spell Timer: Fixed bug that would cause color filters not to apply when you made them. This same bug would also generate errors when a color filter was removed.
- Spell Timer: Fixed cooldown updates when the Spell Timer and Cooldown Timer were both loaded.
- Spell Timer: Fixed resists not being detected in patch 4.1.0.
- Spell Timer: Cast time should update properly again.
- Spell Timer: Tick damage indication using the bar spark. I will extend this to other damage and healing in a later version.
- Spell Timer: Flipping the bar direction.
- Spell Timer: Include the time you have to safely overlap spells in the 'cast time glow' and some other tweaks to it.
- Spell Timer: Raid icons will now be displayed on the optional name tags/headers if those are enabled. They are then hidden on the bars themselves.
- Spell Timer: You can change the location of group headers/labels to top or bottom.
- Spell Timer: A few new default 'Powerup buffs' added.
- Cooldown Timer: fixed bug that would prevent a cooldown from updating when the new time was below 2.99 seconds (read: the value of Advanced Options > Cooldown Timer > Minimum duration).
- Cooldown Timer: A few new hidden cooldowns added.
- Cooldown Timer: Option to hide the frame when out of combat.
- LUI: If you are using LUI, you need this patch to make it work until LUI gets updated for FX-v1.975: [http://www.wowinterface.com/downloads/info19892-ForteXorcist-LUI.html].

### [v1.974.8]

- General: Fixed compatibility with 4.1.0 combat log.

### [v1.974.7]

- Fixed options panel frame not opening when you have the Spell Timer installed, but not the Cooldown Timer.
- Updated Korean translations.

### [v1.974.6]

- Spell Timer: added option to show stacks on the icons.
- Spell Timer: added option to hide frames when out of combat.
- Spell Timer: added option to intelligently adjust countdown text size. This is meant to 'smooth' changes in the width of the text itself and the unit label width, and mostly meant for players that want the duration text on the right side. Enabled by default.
- Cooldown Timer: added a more friendly way to enable the cooldown text on the icons.
- Cooldown Timer: time format on the icons will be the same as on the Spell Timer. This means that you may have to adjust the font size to fit properly.
- Paladin Module: added various optional raid/party announcements, thanks to 'fakeh'.

### [v1.974.5]

- Spell timer bar name labels have a proper fixed height again (same as the bar itself).
- Support for 'special' cast times on the Spell Timer. At the moment 'Improved Steady Shot' is added with a cast time 2x that of 'Steady Shot'.

### [v1.974.4]

- Some fixes to the new Spell Timer layout. E.g. name/spell tags again have a defined width, so long names stay in the bar and don't overlap places they shouldn't.
- Added Sap break/fade messages for Rogues.
- FX now also regularly checks arena enemy unit tokens and boss tokens for buffs/debuffs. If you want to use the arena unit tokens to cast on directly (e.g. in macros), you have to add those to 'Advanced Options > Casting > Additional unit tokens' for best results.
- Permanently removed the Forte_Shard module.

### [v1.974.3]

- Spell Timer icons can now be switched on/off and moved to left/right.
- Spell Timer spell/unit texts can now be switched on/off (e.g. in case you want to have tiny bars).
- Added and corrected a number of ICDs and Powerup Buffs.
- Moved the cap for the 'Standard fade delay' and 'Failed display time' (ghost time) from 10 seconds to 2 minutes. Be careful with this though! Lower is better for performance.
- Removed a few old (and in my opinion unneeded) settings related to the spell/unit name texts and the countdown texts.
- Removed 40 debuffs cap check from the Spell Timer, meaning that targets with over 40 debuffs on them will now have their debuffs removed properly.
- Added advanced option to the Spell Timer to change the duration change smoothing.
- Some Performance improvements.

### [v1.974.2]

- Using the time-based filtering on the Cooldown Timer should now work properly under all circumstances.
- Pet spells that are added to the Spell Timer should be tracked properly now and the Seduction timer should be working again.
- Many small additions and fixes to class modules.

### [v1.974.1]

- Many small corrections to the additions of v1.974.
- FX can now see the difference between the Dark Intent buff and its procc.

### [v1.974]

- Some class modules were updated, mainly the Hunter module.
- A number of internal cooldowns were added to the Cooldown timer.
- 'Highest timers outwards' sorting option now works again when 'Group by Unit' is disabled.
- Added a confirmation dialogue to deleting Profiles and clones.

### [v1.973.1]

- Fixed error in the Druid module.

### [v1.973]

- Changes to the spells in the class modules. Mostly: Paladin.
- Renamed "Skull Bash" and "Swipe" for Druids to include "(Bear)" or "(Cat)"

### [v1.972]

- Fixed problem with the 'Raid Debuff' type in the Spell Timer that would cause them not to show on a quick deselect -> reselect.
- Fixed a few unwanted global variable taints.

### [v1.971]

- Fixed problem with totems not showing up.
- When target/focus is changed the spells that were hidden with 'Hide timers if remaining over' will only re-show if they actually are the new target/focus.
- Timers that were supposed to fade away instantly, like powerup/self buffs, self debuffs and drains/channels, will now always do so again.

### [v1.97]

- First version 'clone-able' Spell Timer! When you create a new clone the settings will be copied from the instance you have selected. They can then be edited freely.
- This version will still use a lot of the original Spell Timer code. A complete Spell Timer rewrite is planned for v2.00.
- Note: I'm not 100% done with the way the animations behave when you change target/focus and 'One maximum' is used. I will smooth this out in the next update. But for the most part you shouldn't notice any difference.
- To further improve the functionality of cloning, there are now a few new options under 'Units' to switch on/off timers more easily.
- Added an option to enable unit name labels/headers independent from switching between spell names and unit names on the bars.

### [v1.966.8]

- Changed Soulstone cooldown at the Soulstone tracker back to 15mins.
- Font size range is now much bigger (1-64).
- Min/Max remaining time and duration settings enabled on Cooldown Timer. Enabling this may still be buggy!

### [v1.966.7]

- Fixed problem that could prevent FX from loading in rare cases.

### [v1.966.6]

- Removed DoT-refresh-duration-with-different-haste-bug fix, because it's no longer needed in 4.0.3. Haste (time between ticks) should now update with refreshes too.
- '- Bear' and '- Cat' will be renamed to '(Bear)' and '(Cat)' for consistency. Your filters will be renamed automatically.
- Option sub-categories are now collapsed by default (basically all but the 'Basic' categories). You can click their header to show/hide them. Mouse over a hidden category to view the options in it. You can disable this behaviour by going to Advanced Options > Options Appearance > Expand all.

### [v1.966.5]

- Small change that should prevent Corruption, SW:P and some other similar spells from falling off too soon. Note for people on the Cataclysm beta: this behaviour is currently fixed on the beta realm, and refreshing these dots again updates haste as well. This means that FX will not indicate the correct duration because it's trying to correct the bug from 'live'.
- Quick fix to 'unknown target' bars staying up where they should have been removed. I added an option under 'Units' to completely hide these bars as well. For more information about the 'unknown target' problem see: [http://www.wowinterface.com/portal.php?id=513&a=faq&faqid=636].

### [v1.966.4]

- Fixed some core problems with the last version.

### [v1.966.3]

- Fixed bug with haste being assigned to abilities that shouldn't receive any.
- Updated DoT-refresh-duration-with-different-haste-bug fix for the 4.0.1 patch.
- The above changes mean that durations of many spells should be more accurate now and not need as much time to adjust.
- Countless changes to the spells in the class modules. Mostly: Mage, Priest, Hunter and Paladin. Still far from finished with all the updates.
- Removed all code related to old Soulstone types, Healthstone types and Shards.
- Reworked the Healthstone Spy and parts of the Soulstone tracker.

### [v1.966.2]

- Countless changes to the spells in the class modules. Still far from finished with all the updates. If your class hasn't received any changes yet, just be patient!
- Cooldowns added to the Spell Timer through 'Customize' will now update their durations properly (for example Metamorphosis and Lava Burst). Note that this only works when the Cooldown Module is enabled too.

### [v1.966.1]

- Countless changes to the spells in the class modules. Mainly Warlock, Death Knight, Druid, Paladin. Still a long way to go!
- Minimum cooldown duration will be set to 2.99 seconds now, so it still shows spells with a 3 second cooldown.

### [v1.966]

- Built for patch 4.0.1.
- Shard Spy and Manager removed.
- Haste mechanics changed. Still working on this one.
- Damage over time refresh/update mechanics changed.
- Made a start with fixing class modules (spells) for this patch, but the modules will be nowhere near complete. Feel free to post missing or bugged spells.

### [v1.965.3]

- Fixed downgrade -> upgrade problem with the Spell Timer "Show Sparks" setting.

### [v1.965.2]

- This is a small code improvement update only. You should not notice any changes unless you had problems with one of the previous versions.

### [v1.965.1]

- Hopefully fixed 'all' errors a number of people were getting.
- Added some LUI-specific fixes. LUI v3 users should also check [http://www.wowinterface.com/portal.php?id=513&a=faq&faqid=628]

### [v1.965]

- Fixed locale file corruption of v1.964.
- Added Clearcasting warning sounds for Mages and Druids.

### [v1.964]

- All Class modules' spells-ids have been updated and they should work much better with Cataclysm now. I've not made any specific changes for Cataclysm yet though. There shouldn't be any problems, but let me know if these changes caused any unwanted effects on the Live (3.3.5) version. Please don't post any spell bugs you encounter in the beta yet.
- Several small fixes to class modules.
- Fixes in the Cooldown module related to the latest changes in Cataclysm.

### [v1.963]

- Works with Cataclysm. I've fixed the Warlock and Death Knight modules so most of their spells get recognized in cataclysm too (using the rank1 spell ids now), but I still have to do this for all other classes. You can add any missing spells for other classes using 'Customize' for now, but I'd wait with that to be honest. I have not changed anything to reflect new spell behaviour etc though! Please don't report any spell bugs that you find in the beta at this time.
- Added an option to change the transparency/alpha of the sparks.
- Added the Twilight trinkets.
- Added option to disable the startup text messages of FX.

### [v1.962]

- Fixed problem with the Curse Client! (right?!?)
- Added Hurricane channel timer.
- Added Water elemental timer (if I got this right...).

### [v1.961]

- Fixed problem with Spell Timer type sorting when 'timers with target' were moved around too.
- Val'kyr Protector should also show up on the Spell Timer now.
- Added back option to disable 'Adapt to one maximum' time for the Spell Timer.
- Fixed rare loading error in the Cooldown Timer. Let me know if fixing this gave unwanted side-effects though, because I'm still not sure how this was even possible.
- Fixed a few errors in the Casting module when the Spell Timer is disabled.

### [v1.96]

- Spell and Cooldown timer options revamped. Mainly changes to the coloring/filtering categories. New options are added and some are either removed completely or moved to the advanced settings. Let me know if I removed any options that you REALLY want to keep using and I'll think about adding them back.
- All Spells that get removed or updated on the Cooldown timer will also update properly on the Spell timer. Support of cooldowns on the Spell timer is still extremely limited without the Cooldown timer installed.
- Added a advanced option for the Spell Timer to change the spell type sorting order.
- Added interface translations for German players.
- Added interface translations for Korean players.
- Spell Timer test bars work again.
- DROPPED frame creation of Soulstone, Shard, Healthstone and Summoning module update for now, considering Cataclysm changes.
- Some options in this version do not work yet. These options are greyed out for now.

### [v1.959.8]

- Fixed loading problems related to changes in most modules. This included /fx resetall not working in the previous version.

### [v1.959.7]

- Fixed Soulstone Tracker error.
- Fixed Val'kyr Guardian timer.
- Fixed stacks (1) showing for some 'powerup buffs' that really don't have any. These are manual fixes to a blizzard bug, so let me know if there's more that need fixing in that way.
- Added Rapture hidden cooldown to the Cooldown timer (Priest module).
- Changed some things in all modules for performance and easier use in the future.

### [v1.959.6]

- Some quickies.

### [v1.959.5]

- Fixed loading problem for non-English paladins.
- Removed and fixed some old talent-specc related code. Talent Spy itself is still disabled though.
- Removed old oRA2 related code.
- Soulstone Tracker module will work with oRA3 now. The number of abilities you can see in FX is still the same (which means that you can see a lot more abilities in the oRA3 interface).
- Healthstone Tracker module cannot use oRA3, so it will only work for people with FX. It will now show the number of ppl with hs vs total number of people that can be tracked. It can also show the division of hs types over the raid and what warlocks can make those.
- Fixed double Eclipse names (blizzard finally fixed the names themselves yay!)
- Some small performance fixes.

### [v1.959.4]

- Added a fix for haste not being used in the Spell Timer under some circumstances. This may not yet fix ALL haste problems though.
- Cooldowns that are included in the Spell Timer should now always show up (under special circumstances they sometimes wouldn't).
- Added back the option in the Spell Timer to temporarily hide timers longer than X time remaining. This behaviour is improved for powerup buffs and raid debuffs. They will not re-appear every time 'something' changes on yourself or your target, instead they will only briefly re-appear when refreshed or removed.
- Temporary hiding powerup buffs and raid debuffs by shift-clicking the icons also work better now. They will not re-appear every time 'something' changes on yourself or your target, instead they will stay hidden until refreshed.
- Drain spells should under no circumstances generate multiple bars now.
- Added Val'kyr Guardian timer.
- Multiple changes and fixes to class modules.

### [v1.959.3]

- Fixed a tiny insy winsy bug in the core.

### [v1.959.2]

- Profile selection and creation will use tabs now too. This makes working with them more intuitive. Original profile area is removed.
- A few changes to some buffs/trinkets.
- Some fixes in the interface itself e.g. regarding tabs.
- Works on PTR too now.

### [v1.959.1]

- Fixed problem with the addon not loading up for people that at some point used the Spell Timer module but now have it disabled.

### [v1.959]

- Background (empty bar) alpha setting for the Spell Timer. The time at which the bars start to blink can now also be changed.
- Maximum bar colour alpha for the Cooldown Timer (so now you can also completely hide the bars).
- A number of spell additions and fixes across all modules (see feature requests and bug reports).
- Small performance fixes.
- You can now also use /fx profile <profile name> to switch to a different profile. This is case sensitive!
- Options interface updates. Right-clicking spell icons will now also fill in the proper filter type, and not just the name of the spell. This should make it much easier to create proper filters. Right-clicking frames and spell icons also sends the options interface to the right frame/clone/instance tab.
- Note that it already supports creating clones as well, and you can actually create Spell Timer clones, but these clones will still use most of the settings from the 'main' instance. It offers the opportunity for me to get some early feedback though, because the interface for working with clones won't change much more. In other words: don't use clones yet unless you're simply curious about how it's going to work!

If you want to update from v1.16 or earlier you'll have to install and load v1.958 first. I'm hoping there's nobody that will need to do this, but you never know. I had to get rid of my compatibility fixes at some point.

### [v1.958]

- Fixed major problem in the glyph detection code... has been slumbering there for a year. Explains a lot of the problems people had with hasted spells not getting any haste on the Spell Timer.
- Frame strata (level) will be switched back to MEDIUM (old value) if you have it set to HIGH currently. Now all frames have an advanced option for their level.

### [v1.957]

- Added advanced options to change the frame strata of the Spell & Cooldown timer frames.
- A few other additions and fixes.

### [v1.956]

- Fixed a Cooldown module bug for Deathknights (new users only).
- A few other additions and fixes.

### [v1.955]

- Ignoring Runes at the Cooldown Timer will now also properly ignore all associated abilities.
- Death Rune type is removed. The bars will keep their original color and glow, but instead the icon will now update to the Death rune properly.
- When the Cooldown timer is loaded you can add any cooldowns you want to the Spell Timer with the customize filter. This is pretty much a quick hack, so use at your own risk! A better version will come.
- Various fixes and additions to the class modules.
- Default Russian Font changed to a font that actually works. Note that the options interface will also switch to this font for old Russian users.

### [v1.954]

- Yeah... fixed retarded lua error for warlocks.
- Feral buff 'Berserk' is now called 'Berserk (feral)' so you can distinguish between that and the weapon enchant.

### [v1.953]

- Fixed update of hasted dots as much as currently possible. Note that I cannot detect the effect of 'hidden' haste buffs (e.g. Improved Moonkin Form, Swift Retribution) until I update the talent spy module.
- The two types of Eclipse should be able to show simultaneously in the Spell and Cooldown timer now. They are called 'Eclipse (Lunar)' and 'Eclipse (Solar)' in all languages now. I still need some ppl to update the locale files.
- Fixed lua error when left-clicking a module frame before the options were opened at least once.
- Fixed lua error related to Bloodworm summon.

### [v1.952]

- Some more fixes!

### [v1.951]

- Some more fixes.
- Fixed and added some more buffs/abilities.
- You can see debuffs on yourself now if you want this (mainly added for arcane blast).
- Added a Blood Worm timer for Death Knights.

### [v1.95]

- Quick fixes to things I overlooked so far.
- Some Performance fixes. e.g Less raid buff/debuff scans and removed cast monitoring of party/raid members in the Soulstone and Summoning modules.
- Added a few spells and trinkets to the class modules.

### [v1.94]

- Fixes for patch 3.3. Mainly (only?) support for hasted dots.
- Fixes to some outdated code in the core modules which could cause lua errors (not related to 3.3).
- Added a few spells and trinkets to the class modules.
- No more, no less!

### [v1.93]

- Quick fixes!

### [v1.92]

**Note:** A number of options are moved to the Advanced category.

- Advanced option added for the Cooldown Timer to set the minimum full duration the cooldowns must have for them to show up at the Cooldown Timer (For now you could set this to 10seconds to ignore runes and their associated abilities).
- Cooldown type added to the Spell Timer. Currently only for a very selected number of spells.
- Fixed problem with the options panel when both Spell and Cooldown modules were disabled.
- Summoning assistant will show up again properly.
- Fixed a bug with timer bar grouping (unit # assigned improperly).
- Use custom backgrounds for the Spell & Cooldown Timer. (still incomplete, but good enough for people that really want to use this)
- Time format of Cooldown/Duration left messages fixed.
- Shaman Totem code updated. Each totem type has it's own type/color now, which can be changed. Totems that were already up when you loaded the game should also show up properly now.
- Fixed drain spells not showing when the cast target guid was 'unclear' to the addon.
- Once again fixes to the custom filters.
- Cooldown 'scale time tags' will be drawn above bars, and below icons again, instead of behind the bars.
- Fixed problem with a few settings not applying properly when switching profiles.
- 'Smoothed out' Spell Timer behaviour. E.g. No more weird up-down time/highlight switching on casts. Only new or newly cast spells get highlighted, the rest will regain in time smoothly to attract less attention. Stacks of self-casted spells should also no longer switch. 'Fall-off effect' is now smoother for groups with unit name labels. And you can of course still target away while casting and the timers will still show up properly! The current version will be a bit more sensitive to wrong spell data (mostly durations) in the class modules, so please report any weird behaviour.

### [v1.91]

- Knock-back of drain spells fixed.
- Some fixes involving Talent Switching.
- Fixed bug that could prevent the addon from loading properly.

### [v1.90]

- A number of spells have been added and fixed.
- A number of other small fixes all around.
- Revised some of the customization code so the timer changes will always update instantly.
- The visual parts of the Core, Spell Timer and Cooldown timer have been rewritten. You should not notice a lot of changes, but keep your eyes out for 'new' bugs.

**Note:** some of the new options you will find do not work yet.
Important: You will keep all your settings from an older version, but once updated to v1.90 you can not 'downgrade' back to a pre-v1.90 version without loosing a lot of settings. Be careful with that.

### [v1.16]

- Finally fixed the problem with unwanted 'other debuffs' showing up if you made a custom filter with its name, regardless of what type/action. Sorry it took so long! :P

### [v1.15]

- Some finalizations to the new filters and filter lists
- The usual fixes

### [v1.14]

- The customize filters have an extra value where you can select the type of spell that needs to be affected by the filter. This should make the customizations much more powerful.
- In addition, the customize options can now give an overview of all the changes you made!
- The '/fx position' command is replaced by '/fx reset' and will now reset all option-frame related settings like position, scale, columns and lock. (the old command still works btw, but does the same as the new command now)
- Heal Over Time spells have their ticks displayed (default is 3 seconds, so this may not be correct for all spells yet)
- If you attempt to cast a spell that's on cooldown, the Cooldown Timer will try to get your attention and show you where the spell is on the timer.
- Rogue module updated to work more as intended. I'll need your input to check if it's all working correctly though.
- Many small changes to all other class modules.
- Display of internal trinket cooldowns no longer require the spell timer to be active.
- Fixed some problems with icon grouping in the cooldown timer.

As always your settings should be converted to their new formats without you even noticing it!

### [v1.13]

- Fixes in and additions to the paladin module
- Small fix that will prevent dot listening before your combat log has actually started to work. It will also disable dot listening, since I'm not sure if the first fix is enough. You can re-enable it in the options.

### [v1.12]

- You should no longer get an error the first time you update (this was a v1.11 problem only) :P
- Secondary Splash Icon will now properly use the alpha setting in the header, and the old setting is removed.
- Some Hunter module changes
- Some other Quick fixes!

### [v1.11]

- All Self Buffs (yes buffs only, no debuffs or items) that are set to 'show' or 'color' in the custom filter will show up as a Cooldown Icon or Spell Tmer with the type 'buff'. Before only buffs pre-set in the module code could be added.
- Fixed Stealth/Prowl Cooldown to only show when you leave stealth.
- Fixed the artificial cooldowns of multiple paladin spells that cannot be used within a certain time of each other.
- Preset colours for the module options. This should help not to edit the wrong module by accident. You can disable this again from the options appearance settings. I may still change the colours a bit.
- A transparency setting is added to all module frames.
- Attempting to drag a locked frame will no longer cause you to 'click' it.
- The Secondary Splash icon now has its 'own' options for clarity. Note that it still uses the type/filter settings of the Cooldown Timer.
- You can use a custom tag on the spell timer bars. This is still very basic/limited atm, but good enough for now.
- Many small class module fixes/changes

Although marked as release now, I still keep adding new things that need to be tested. So check back regularly for updates.
