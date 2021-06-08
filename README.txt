=================================================================================================================
    Better Ships v1.0

    By Delta of Isaire

You are free to use any part of this mod for your own mods/works so long as you credit me for the original creation :)
=================================================================================================================

This mod does 4 things:
    > Rebalance/buff Ordnance Point (OP) capacity of ships for a more FUN amount of OP.
    > Tweak the Deployment Point (DP) cost of a few ships for better balance after the OP changes.
    > Overwrite vanilla goal variants with versions that account for new OP capacity and are less terrible.
    > Reduce randomness of autofitting, so that ships try to adhere to goal variants more closely.

This mod does NOT apply to Omega ships for now, except for reduction of autofit variation, because Omega's are fairly overpowered and I don't have enough experience with them yet.



Ordnance Point rebalance
------------------------
For most ships, OP capacity changed to equal the sum of:
    > Maximum number of Vents (without skills), i.e. 10/20/30/50
    > Maximum number of Capacitors (without skills), i.e. 10/20/30/50
    > OP cost of Integrated Targeting Unit, i.e. 4/8/15/25
    > OP cost of Heavy Armor, i.e. 8/15/20/40
    > 0/5/10/15 OP for Fourteenth Battlegroup (XIV) modification
    > 5 OP for every small gun mount (OP cost for average weapons like IR Pulse Laser and Light Assault Gun)
    > 4 OP for every small missile mount (standard OP cost of small missiles)
    > 10 OP for every medium gun mount (OP cost for average weapons like Heavy Autocannon, Pulse Laser)
    > 10 OP for every medium missile mount (standard OP cost of medium missiles)
    > 20 OP for every large gun mount (OP cost for average weapons like HIL, Autopulse Laser, HAG, Mark IX)
    > 20 OP for every large missile mount (baseline OP cost of large missiles)
    > 10 OP for every fighter bay

Composite/Synergy/Universal mounts are considered gun mounts for OP calculation.

Weapon and Fighter slots with built-in non-removable weapons are not counted (e.g. Flak Cannons on Monitor, Mining drones on Venture).

For Civilian ships that are not combat-freighters (so real non-combat ships), the new OP capacity does not include the bonus for ITU and Heavy Armor.

For Ox and Salvaging Rig the OP capacity is unchanged for balance reasons.

For Guardian the OP capacity is also unchanged, because the new calculation would result in a significant loss of OP (375 vs original 450) and this thing deserves to be good.


>>> On average this results in a 30% increase in OP capacity compared to vanilla. But note that some ships benefit (much) more than others.



Deployment Point tweaks
-----------------------
Radiant - 60 (was 40) because it is at least as good as Paragon.
Guardian - 60 (was 40) because it is at least as good as Paragon.
Colossus Mk.II - 12 (was 9) because it is no longer held back by low OP.
Colossus Mk.III - 12 (was 8 ) because it   is no longer held back by low OP.
Scarab - 10 (was 8 ) because Temporal Shell makes it stronger than Tempest and Shrike.
Scintilla - 15 (was 12) because it is easily as good as a Drover.
Afflictor - 10 (was 8 ) because it's a better Shade.



Reduced randomness of autofitting
---------------------------------
Is done by setting "autofitRandomizeProbability" to 0 in all relevant .faction files (in /data/world/factions).

This tweak means AI ships adhere fully to goal variants, unless the required blueprints aren't available because either (1) the faction doesn't have those blueprints at all or (2) the game randomly decided that, for fitting this particular ship, certain blueprints aren't available. So it doesn't completely remove autofit variation, but greatly reduces it.
