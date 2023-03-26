# Keeping the Bow of Light

The Bow of Light ("**BoL**") is an unbreakable energy-firing bow that is supposed to only be available during the last battle with Ganon's final form (Dark Beast Ganon). Using [IST](/ist/README.md), you can transfer it back to one of your previous saves, with no other permanent effects to your save file.

## Theory

You will generate enough IST offsets to cover the Bow of Light plus any items (Arrows, unsellable Armor, Key Items, etc.) that you cannot reasonably remove from your inventory during the final Ganon battle.

Once the Bow of Light has been acquired, you will drop/use all other Inventory items, and then reload a previous target save. Due to the broken IST slots, the BoL gets transferred (temporarily) as well.

Finally, after some Inventory clean-up, you will be able to transfer the BoL back to your main save.

## Preparing your manual save

Ensure your save file has at least one free bow slot, and manually save. From this point on, stick to autosaves only.

## Preparing your autosave

You will need the house in Hateno Village and a free bow mount in it (partial completion of the _Hylian Homeowner_ side quest). You should also get Myahm Agana Shrine as a fast travel point.

Since you'll have to defeat Calamity Ganon to get to the BoL in the first place, here are some things you might want to do to prepare:

- Free all Divine Beasts if you don't want to fight any Blight Ganons in the castle.
- Grab any powerful equipment from places like Hyrule Castle that you want to have.
- Buy as many arrows as you want.
- If you have the Travel Medallion, you can place it close to the Sanctum entrance for a quicker castle ascent.
- Cook as many hearty/mighty/tough meals and elixirs as you want.

Redeeming some Key Items can make the fight easier, and maybe even reduce how much offset you'll need:

- Redeem as many Spirit Orbs as you can. If you have a multiple of 4, the slot will disappear from your inventory.
- Spend Korok Seeds to get equipment slot upgrades. If you can spend all of your seeds this way, the slot will disappear from your inventory.
- If you have 3 of any of the Champion's Emblems, redeem them at their appropriate Divine Beast to remove them from your inventory. Don't attempt the Blight refight, just leave immediately.


## Reducing the inventory

You want to minimize the number of items in your Inventory before you generate an autosave outside the Ganon battle. In most cases, that means either dropping them during the Dark Beast Ganon fight, or making offset slots to cover them. Some items should be sold before making the autosave (don't sell them yet, you'll need them to make offset). The amount of offset you need depends on your inventory, but this is how to calculate what you need:

1. Weapons appear to the left of the BoL, so we ignore these entirely.
1. Most bows will also appear to the left of the BoL, but you need to make 1 offset for the BoL itself.
1. Arrow stacks cannot be removed during the fight, so make 2 offset for every stack.[^s500+]
1. Shields can be dropped in the DBG fight, so don't make offset for them.
1. Armor always duplicates, so make 2 offset for every piece of unsellable armor you have (as well for any sellable armor you explicitly want to use in the fights). Sell all other armor.
1. Materials can be dropped during the fight, but this takes time. Sell all materials (except fairies), and don't make offset for them.
1. Food can be eaten at any time, so don't make offset for it. You should sell any high-quantity roasted and frozen ingredients to save time later.[^icfood]
1. Key Items cannot be reduced during the DBG fight, so make offset for each slot. You need to make 2 offset for the following[^s500+]:
    - Korok Seeds;
    - Spirit Orbs;
    - Champion Emblems;
    - **Upgraded** Champion Powers, if you obtained them legitimately on this file. (Upgraded champion powers that you only have because you transferred them in from another save will not duplicate, and you can count them once.)

[^s500+]: If a stack is at 500 or more, it won't duplicate, and you only need 1 offset for it. However, be careful when doing this with arrows. If you use enough of these arrows in battle that the stack drops to _below_ 500, it will duplicate and you'll be down an offset slot. I recommend only doing this with arrow stacks at 700 or more.

[^icfood]: You should also sell any meals/elixirs with corrupted quantities, if you made those.

## Making the autosave

1. Make the amount of offset you calculated above. You can overshoot slightly if you're unsure. From this point on, **do not**:
    - Load any save file.
    - Die. If you die, you have to close and reopen the game, and remake the offset.
    - Pick up a new type of arrow, if you didn't already have all 6.
    - Obtain any new unsellable armor.
    - Complete any Shrines.
    - Uncover a hidden Korok, if you have no Korok Seeds.
1. Sell all armor that you can (except pieces you're saving for the Ganon fights).
1. Sell all materials except fairies.
1. Head to the Sanctum, being sure to collect at least one autosave along the way.

## Ganon fights

During these fights, you can freely make any use of weapons, bows, arrows (if you don't fall foul of [^s500+]), shields, and food.

1. Enter the Sanctum and defeat any Blight Ganons that show up there.
1. Defeat Calamity Ganon.
1. Enter the Dark Beast Ganon fight and collect the Bow of Light.
1. Drop all bows to the right of the BoL. There should be none if you never sort your Bows tab.
1. Drop all shields.
1. Use all fairies. If you have other materials, jump off your horse and drop them all.
1. Eat all food.
1. Reload your last autosave.

You will now have an inventory with the Bow of Light in it, and a game world state with no Dark Beast Ganon spawned on Hyrule Field. However, you'll probably also have a whole bunch of duplicated arrow stacks, armor pieces, and Korok Seeds.

## Removing duplicated items

The next step is to _nuke_ the inventory, by getting a save file with no inventory contents at all. This happens when your offset is equal to, or greater than, the number of inventory slots you actually have (`mCount < 1`).

1. Head to Link's house in Hateno village.
1. Attempt to put the BoL on the bow mount. It will appear to snap back into Link, but the mount remembers what you tried to do.
1. Leave the house, and run to the other side of the bridge over the gorge to despawn the mount entity.
1. Run back again. The mount should now have a copy of the BoL on it.
1. Drop everything you possibly can from your inventory.
1. Verify that mCount is low enough:
    1. Unpause and pause again. If your inventory goes completely invisible, you have exactly enough offset. Don't pick anything else up, and skip to the next step.
    1. If you can still see your inventory, pick up one weapon and pause again. If this turns your inventory invisible, or the weapon appears to the right of your Key Items, you also have enough. Don't pick anything else up, and skip to the next step.
    1. If the weapon sorts to the correct position, you don't have enough offset. Gather materials and make some more, then try clearing out your inventory again.
1. Run to Myahm Agana Shrine, or the central street of Hateno Village, for an autosave.
1. When it completes, close and reopen the game.

You should now have a near-empty inventory, with nothing in the first 6 tabs. Your Key Items might contain Champion Powers, or a Travel Medallion, but all duplicated slots will have disappeared entirely.

## Final BoL transfer

1. Head back into Link's house and pick up the BoL off the mount.
1. Grab a one-handed weapon and a shield to make K+1 arrowless offset (one for each Key Item you still have, plus one for the BoL).
1. Clear out your inventory again. If you can drop something, drop it.
1. Reload your manual save to transfer the BoL into it.

Pause and check your inventory. If you see the BoL there, **unpause, pause again** and manually save. Close and reopen the game to clear offset.


## Advanced method

There is an [advanced method](Keeping%20the%20Bow%20of%20Light%20%28advanced%20method%29.md) that uses Prompt Entanglement to steal the BoL more quickly and safely.


