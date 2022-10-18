*****************************************************************
     The Elder Scrolls III
          MORROWIND:
      Lichcraft2 Patch
            V 2.00
	by Madgamer98
*****************************************************************
Contents:
1. Installation
2. Patch Changelog
3. Additional Patch Credits

*****************************************************************
     1. INSTALLING THE PLUGIN
*****************************************************************

To install the patch, unzip the .esp into the Morrowind/Data Files directory
overwriting vn_lichcraft2.esp and vn_lichcraft2_alt.esp.

This mod requires both Tribunal and Bloodmoon to be installed.
It also requires the base lichcraft 2 mod files.

There are 3 .esp included with this plugin.

vn_lichcraft2.esp - default. When you become a Lich, you lose the ability to use certain clothing slots 
vn_lichcraft2_alt.esp - Alternative. When you become a Lich you may use any equipment slot, but your original appearance is forever lost.

vn_lichcraft2_VH_Patch.esp - Compatability Patch for Vampire Hunger to handle Attribute Fortification refresh when possessing a host.
Can be used with the default or alt lichcraft 2 esp

*****************************************************************
     2. Patch Changelog
*****************************************************************

30 November 2021 Madgamer98 Lichcraft2 Patch 1.0:
     1. Opened and saved/Recompiled all mod scripts which fixed the ritual breaking with potions not being drank.

     "So strange thing. I was opening up the files to see what was wrong with the fix files during the ritual and why the potions were acting up
     (they wouldn't be consumed immediately after clicking yes in the message box and the ritual would fail the second you put on the Phylactery)."

     "it seems that it will fix itself by just opening the 3 potion scripts (vn_lichpotionscript, vn_lichpotionscript_vamp, vn_lichpotionscript_failed)
     and re saving them then saving the .esp file. I also resaved the vn_lichritual script as well and then tried the ritual with the fixed esp.
     This allowed me to consume the potion correctly after clicking through the message box and the ritual worked."

     "I'm wondering how many other scripts are wonky and aren't working correctly. Not sure why this even fixes the issue but it does for me at least.
     I've gone ahead and re-saved all my scripts in my esp file just in case."

08 August 2011 Claviticus Lichcraft2 Patch Beta 2:
     Here is the next version, I finished cleaning all the scripts with my tool, and MWEdit. (They still need some manual formatting, but they should be free from syntax errors now. I also removed the reference to Book Rotate, sorry about that little slip up).
     As for the next update:
     1. I'm going to fix the disguise spell. (Right now it has some issues involving the lich crown, and crown of souls. It needs a few MenuMode checks, etc,.)
     2. I'm probably going to go ahead and make separate bounties for each form. (I could probably do this without adding extra vars, but, it's just easier to track\swap if I do.)
     3. More script fixes. (Mainly finishing up the formatting.)
     That's about all I have planned so far, I wanna look into the balance code, there were some pretty harsh penalties described in the scripts, but in-game I'm not really seeing them. (For example, ppl are supposed to really dislike me, even in human form, I think, but I have 100 disposition with most people I meet, despite low personality stats, etc,.So I'm just going to make sure everything is working as intended..)

03 August 2011 Claviticus Lichcraft2 Patch Beta 1:
     1. Tons of script errors involving the use of reserved keywords as local variables, ie, float random, long position, both of which are scripting commands, etc,. (I made too many misc fixes to list them all, but it was all minor stuff, like, if ( doonce = 0 ), was changed to the proper if ( doonce == 0 ), etc,.)
     2. Crown of Souls: This was breaking for me, throwing expression errors, etc,. I fixed that, and a few issues with it's OnEquip code, it also had some issues with it's soul eating code, ie, ( RemoveSoulgem "soulgem_type" count ), count is invalid for this function, according to MWEdit anyways.
     3. There may have been a bug that could cause you to miss levels of powers(ie, you get sorcery level 2, skipping level 1), I haven't really tested this out, but the code didn't look very reliable, so I updated it.. (Can't really call it a fix, since it may have been fine, but it's probably better now, at any rate.)
     4. Fixed the "Reduce Notoriety" greater power, it reduces the bounty on your (disguised) human form, however, if cast it while in lich form, it basically wasted a days use and didn't apply the bounty reduction. Now it does, your human form bounty is properly reduced no matter what form you are in when you cast the spell. (I'm sure this is what the author intended, since the lich bounty is hardcoded to be at least 8,000, so reducing it would be kind of pointless since it can never go below the hardcoded limit.)
     6. Removed lot's of debug messages. (ie, body check NULL, etc,.)
     7. Made a few changes to the Lunar Chaneller, it seems to be working properly now. (Before it would sometimes say, you can do the power ritual on day 120, and then, when day 120 came around, it switched to day 140(or whatever), causing the ritual to fail on day 120(day 119 at 11pm technically, since you start the ritual one hour before midnight on the night of the full moon.. Yeah, it's confusing..)


*****************************************************************
     3. Additional Patch Credits
*****************************************************************

Madgamer98
     That's me!
     This Lichcraft2 to fix additional issues that still persist. Built off of Claviticus' patch


Claviticus
     Lichcraft2 Patch Beta 2.7
     Put together a patch fix for lichcraft2
     03 August 2011 - Claviticus published Patch Beta
     06 August 2011 - abot provided improved scripts though untested ingame
     08 August 2011 - Claviticus published Patch Beta 2, but it's unclear whether abot's scripts have been implemented or not


Original Readme Below:
*****************************************************************
     The Elder Scrolls III
          MORROWIND:
      LichCraft Plug-in
            V 2.03 (Final?)
	by VenomByte
*****************************************************************

Stay up to date on LichCraft and other mods by VenomByte!
http://lichcraft.silgrad.com 

Contents:
1. Installation
2. Playing the Plug-in
3. Release History/Mod info
4. Known bugs
5. Credits
6. Contact
7. FAQ/Other notes

NOTE: I will be putting an online FAQ for LichCraft on my website (see above).
There is far more to this mod than I can possibly remember to write down here.
So any questions, check the site or email me!

*****************************************************************
     1. INSTALLING THE PLUGIN
*****************************************************************

To install the plug-in, unzip the files into the Morrowind/Data Files directory.
This mod requires both Tribunal and Bloodmoon to be installed.

NOTE: If you are also running the Mad Leveller, make sure it is loaded AFTER LichCraft. Additionally, DO NOT use
 the Mad Leveller LichCraft fix. It is no longer compatible, or necessary.

There are two .esp's included with this plugin.

vn_lichcraft2.esp - default. When you become a Lich, you lose the ability to use certain clothing slots 
vn_lichcraft2_alt.esp - Alternative. When you become a Lich you may use any equipment slot, but your original appearance is forever lost.


*****************************************************************
     2. PLAYING THE PLUGIN
*****************************************************************

From the Morrowind Launcher, select Data Files and check the box next to the "Lichcraft.esp" file.

This plugin was designed as an alternative, expanded take on the Lich experience originally offered by Illimunated Order.
It is a standalone plugin.

To start your adventure, look in the secret library of Vivec for a certain
 book on Necromancy...

*****************************************************************
     3. Release History/Mod info
*****************************************************************

To check if a later version has been released, please visit www.freewebs.com/lichcraft

---------------

v2.03
- Respawning NPC's should no longer have uber-health
- removed body script messages. Again :)
- other changes I didn't write down and can't for the life of me remember... 

v2.01
- Fixed raise dead script
- removed body script messages
- corrected initial spell assignment

v2.0
A multitude of new features.
- Recruit greedy mages to act as your followers.
- Make your mage followers pray to increase your powers
- Build your own Lich Lair, anywhere you choose.
- Specialise your Lich in the 'Lich Avenues' - Necromancy, Psionics, Sorcery, and (for Vampire Liches only) Vampirism.
- 40 unique powers available in the above avenues
- Raise over 20 different undead creatures - assorted skeletons, bonewalkers and ghosts.
- Become a Vampiric Lich and suck the life from the people of Morrowind to feed your powers.
- Lots more I can't think of right now!

v1.x
Lots of beta releases. Details withheld :)


v1.0 - public release!
FOllow a series of tasks and undergo the ritual necessary to become a Lich, a powerful magicka-weilding undead.

Lich features include:
- level-based bonuses to magicka related skills and attributes
- create your own spells of almost unlimited power
- a new way of creating your own enchantments. 100% sucessful.... but not without it's price
- retreat to your phylactery when mortally wounded, and live to fight another day
- disguise your true form to interact with the world as normal.... but you can't sustain this for long
- various other bonuses and penalties

Be warned however: Becoming a lich is a physically draining and irreversable process.


If you're already a lich via Illuminated Order, you'll need instead to type in the console
'startscript, vn_ordercheck'
This will also add a phlyactery to your inventory.


*****************************************************************
     4. Known bugs/Compatability issues
*****************************************************************

The phylactery and the Lich lair only work in cells from Morrowind, Tribunal or Bloodmoon.
Don't use them in cells from other mods.

You can't become a Lich if you're level 80 or over. Seriously... why not just start a new character? The experience
 will be so much the better for it. Or perhaps I should just whack uber-level players down to level 1 on completing
the transformation, eh?

If you're using the Mad Leveller, make sure it is loaded AFTER LichCraft. Additionally, DO NOT use the Mad Leveller
 LichCraft fix. It is no longer compatible, or necessary.


*****************************************************************
     5. Credits
*****************************************************************

TheLys
- wrote the original Lich script, an invaluable starting point for this mod

Charles J. Devito (rhe1@gte.net) / LDones (ldones@hiredgoons.net)
- for the original Lich ideas taken from Illuminated Order. As well as many of their scripts that have been 
borrowed to some extent.

GhanBuriGhan
- for Morrowind Scripting for Dummies. I couldn't have coded a tenth of the script in this mod if I hadn't had
this as a reference. (Or perhaps I could, but it'd have taken ten times longer)

TheOneWriath
- for all the lore on Liches, without which this mod wouldn't be what it is. And likely wouldn't have even gotten off the ground.

Cj Campbell
- for originally hosting the mod on www.brimd.com/lichcraft

Cortex
- some of my key scripting concepts were inspired by the techniques used in VE.


tsbasilisk, reffa, and everyone wlso who is/was involved in testing or brainstorming on this mod.
You know who you are!



 --- RESOURCES: ---

 --- Modders who've created resources especially for this mod: ---

Luminar Nightblade 
- Lich skeleton texture & most things in the new Phylactery interior (including the phylactery itself).

[Someone who's name I cant seem to find. Sorry!]
- Visionary globe, plus moon phase predicting device.

Veryade Athan
- Lich Lair, plus various other bits and pieces.
 

 --- Other modders whose work I've used: ---

MarcusX
- Skeleton crown models

Igor Pavlov
- Gothic Gear (some skeleton weapons and capes)

HopperFly621 & Calishan
- physiqued capes

Michael 'HelioS' Bennett
- various weapons from assassins armory (plus a robe)

Carnithus (http://www.angelfire.com/empire2/innercrypt/)
- various armors from the Armamentarium

Someone else who's name I can't find!
- Onyxwood staff teaser

Dark Baron
- Skeleton mage robe (red)

MP*Canus
- Telvanni mage robe worn by undead sorcerers

Joel Braddock (a.k.a. Mantodea)
- Daedric Priest robe, used by a certain undead follower.

ModMan
- Spirit Stone mesh/texture from the infamous gempack

Slategrey
- for the Lightblue kai globe model which I've 'borrowed'.

Cait
- For the chicken model


Okay, I think that's all :)


*****************************************************************
     6. Contact
*****************************************************************

To contact me for whatever reason (suggestions, bugs, etc) email:

adesignforlife@gmail.com

or message me ('VenomByte') on the ES forums.


*****************************************************************
     7. FAQ/Other notes
*****************************************************************

F.A.Q

1) Can a Vampire become a Lich?
Yes, you can. You follow the same process but with a different potion. As a Vampiric-Lich you cannot use normal
restore health or magicka effects, but there are new ways to gain them...

2) Can I be cured of Lichdom?
No. The process is completely irreversable.

3) Why can't I pick up the book on Necromancy?
That bug has been fixed. You can now.

4) Where can I find Adamantium Ore?
For this, and various other 'How do I' and 'Where is' questions, check the spoiler skull in the census and
excised office in seyda neen

5) Do I take on someone's appearance when I possess them?
No. You remain a skeleton, and your disguised form remains as before. Effectively, you take on only thier physical
attributes - strength, speed, agility, and endurance.

6) Can I enter the Phylactery in any way other than almost dying?
Remember, the phylactery is a 'net' to catch your soul. It's not a retreat you can hop off to when you feel like it.
Previously, the answer to this questions was 'no'. But now there is a way. There is a unique spell in the Avenue
of Necromancy which allows you to fake your own death. If you're lucky, you might recieve this from a power ritual.

7) So hang on... what exactly IS a phylactery then?
When someone becomes a lich, their body dies, and their soul is transferred to a magical container. This container
is the phylactery. It houses the soul of the lich. The Lich may then animate its corpse, and go about its business
as if it were alive (well, as much as a corpse can). Should the Lich be 'killed', it's soul does not pass on to the
 next world, but instead returns to the phylactery, where it can reanimate its body and return to the world. 
A Lich is destroyed if it's phylactery is ever broken, wherever the Lich's animated corpse might be at the time.

8) What's the difference between your lich and the type you can come via Illuminated Order?
Far too many to list.

10) Will there be an Oblivion LichCraft?
Yes. If i turn out to get addicted to Oblivion too.


Other Notes:

*SEMI SPOILER*
See the Lich Crown? There's rather more to it than meets the eye.
