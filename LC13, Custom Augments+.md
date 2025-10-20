# LC13 Prosthetics Surgeon Update

## *Currently, The Prosthetics Surgeon is by far the least complex role in the City Modes. They have no progression, no ability to customize or personalize their products, and once they sell something to you. You have no reason to come back to them, since you can’t have all that many prosthetics. Plus they are expensive and situational\! So, With this update I am planning on giving the Prosthetics Surgeon a new product which has plenty of customizability and progression\! Along with a mini-update to workshops.*

# New Machine: Augment Fabricator

*This is a machine that can be found in the Prosthetics Surgeon office. You can only use it if you have the ID with the correct access. Once you click on it, it will open up a menu which will let you start creating your custom augment.*

## Template

When you start creating an augment, you will need to select what kind of template you will start out with. Templates have 2 mechanical adjustable properties, Form and Rank. Then there are a few ways you could personalize your augments\!

**Form**  
*Form will determine the appearance of the outfit, and other attributes of it. Like fabrication cost, Base EP, and if it can be upgraded. Also, the form will affect the appearance of the augment when it is attached, or when it’s in its compact state. Here are some examples of possible forms:*

| Form Name | Base Cost | Base EP | Other Effects |
| :---: | :---: | :---: | :---: |
| Internal Prosthetic | 200 ahn | 2 | You need to have at least one negative effect. |
| Tattoo | 100 ahn | 4 | Unable to get negative effects, and reduce your attributes. (-4, \-8, \-12, \-16, \-20) |

**Rank**  
*There are a total of 5 Ranks which determine how much Base EP the augment has. Where it gets extra EP equal to \[Rank\*2\]. However, at ranks higher than 1 the augment gets an attribute requirement (40, 60, 80, 100). Also, the base cost will be increased the same way the Base EP is increased.*

**Flavor**  
*You are able to adjust/change some aspects of the augment to make them more personalized to you\!*

1. *Name*  
2. *Description*  
3. *Primary Color*  
4. *Secondary Color*

## Effects

They are the main meat of the augment\! They are small parts that can give strengths in the form of passive buffs, add effects to your attacks, or even give you new abilities. However, each effect has an EP cost, which makes you consider which ones you want to add to your augment. You can increase the amount of effects you can add to your augment, if you attach effects with a negative EP cost. Warning, these effects give you small weaknesses. Also, each effect you add to an augment will increase its cost by a small amount. 

Extra notes, Some effects are \[Repatable\] which means you can spend extra EP to enhance the effect. With **X** symbolizing which effects are enhanced by repeated addition. Some effects could also be variants of other effects, which is marked down with “**\[\]**”.

**Sales**  
At the start of the round and every 20 minutes, the fabricator will undergo a market change\! Which will cause 20% of the listed effects to be on sale. The possible sale values are: 25%, 33%, 40% and 66%. Only 2 effects can possibly have a 66% sale. Along with that, another 10% of the listed effects will be marked up which will increase their cost. The possible markup values are: 25%, 33% and 40%

**Extra Notes**  
The Protestics surgeon will be able to see all of the effects on an augment by examining them.

There will be a tool which lets the prosthetics surgeon remove augments from the person.

Make statues effects last for 10 seconds, and when a new is added check its stack. If it is higher then the current stack you have, replace it and reset it? (Need to think about this more…)

Here is the list of all current effects:

| Effect Name | Ahn / EP cost | Effect Description | Properties |
| :---: | :---: | :---: | :---: |
| **Reactive Damage Effects** *These effects give you some sort of effect when you take damage* |  |  |  |
| Turbulence \[X\] | 200 ahn / 8 EP | Gain a new ability, “Turbulence” While “Turbulence” is active, take 50% less damage from RED and BLACK damage. However, take the remaining amount of damage as SP damage. You are able to toggle “Turbulence” by pressing the ability button. |  |
| **Attacking Effects** *These effects give you some sort of effect when attacking an enemy.* |  |  |  |
| Weakness Exploit \[X\] | 50 ahn / 4 EP | When attacking a target, if their resistance to your damage type is their greatest weakness. Inflict **Y** Fragility to them. **Y** being the damage type you are hitting them with. This has a cooldown of 1 second. |  |
| Extendo Arms | 300 ahn / 10 EP | Your melee weapons gain \+1 range |  |
| Throwing Master \[RED\] | 25 ahn / 2 EP | When you throw your weapon, it will deal an extra 25 \* X RED damage  | \[Repeatable, Max of 3\] |
| Throwing Master \[WHITE\] | 25 ahn / 2 EP | When you throw your weapon, it will deal an extra 25 \* X WHITE damage  | \[Repeatable, Max of 3\] |
| Throwing Master \[BLACK\] | 25 ahn / 2 EP | When you throw your weapon, it will deal an extra 25 \* X BLACK damage  | \[Repeatable, Max of 3\] |
| Retractable Weapons | 25 ahn / 2 EP | When you throw your weapon, after it hits a foe it will retract towards you. (Has a cooldown of 40 \- X\*10 seconds) | \[Repeatable, Max of 3\] |
| Lucky Star | 50 ahn / 4 EP | When you perform a melee attack, there is a 10% chance to perform a critical strike, dealing 50% more damage. However, when you take damage, there is a 5% chance that you will take critical damage and will take 50% more damage from that damage. |  |
| Burning Man | 50 ahn / 4 EP | At 30+ Burn, When you attack a foe you will do an AOE which is most likely to kill you both. When you take damage at 10% or less HP, gain 30 BURN. (Has a cooldown of 30 seconds.) |  |
| **Execution Effects** *These effects give you some sort of effect when executing an enemy.* |  |  |  |
| Adrenaline | 50 ahn / 4 EP | On kill, gain 2 Strength |  |
| **Status Effects** *These effects interact with status effects in some way.* |  |  |  |
| Tremor: Chain \[X\] | 50 ahn / 4 EP | When attacking a foe with 5+ tremor, convert all tremor on target to Tremor: Chain. (For every 5 Tremor the user has, Deal 10% less damage.) (Has a cooldown of 30 seconds) |  |
| Tremor: Decay \[X\] | 50 ahn / 4 EP | When attacking a foe with 5+ tremor, convert all tremor on target to Tremor: Decay. (For every 5 Tremor the user has, Take 10% more damage.) (Has a cooldown of 30 seconds) |  |
| **Ability Effects** *These effects give you some sort of ability, like a skill book. However, these abilities are not toggles, and do something when used.* |  |  |  |
| Grappling Hook \[X\] | 150 ahn / 6 EP | You gain a new ability called “Grapple” This causes you to select a location (Pointed spell), Where you will then fire a grappling hook projectile. Upon hitting a target or reaching the target location, you will throw yourself towards that location. In order to fire the grappling hook, you will need to spend a charge, which you gain 1 every 10 seconds. And can hold a max of 3 |  |
| Weapon Sheaths \[X\] | 150 / 6 EP | Gain a new ability, “Sheath” When activating this ability… If you are currently holding a weapon, store it inside of you. If you already were storing a weapon, instantly equip that weapon. This ability has a cooldown of 10 seconds. |  |
| Consuming Augment, **\[\]** \[X\] | 100 ahn / 4 EP | You gain a new ability called “Consuming Augment” When you use this ability, you are able to select a dead simple mob corpse right next to you. (Pointed spell) Once you do, you will gib that corpse and gain something depending on the effect’s **\[\].** This ability has a cooldown of 40 seconds. **\[HP\]**: Gibbing a corpse will cause you to heal 25% of your max HP **\[Protection\]**: Gibbing a corpse will cause you to take 40% less damage from all attacks for 30 seconds. **\[Strength\]**: Gibbing a corpse will cause you to deal 40% more damage with your attacks for 30 seconds. | If the user has other \[Consuming Augment\] effects, all of their effects are added to the same ability. |
| **\[\]** Mark \[X\] | 100 ahn / 4 EP | You gain a new ability called “Mark Target” This causes you to select a target (Pointed spell), who will become marked by you for 30 seconds. (You can’t mark yourself) The effects of the mark are determined by the effects **\[\].**   This has a cooldown of 1 minute. **\[Commander\]**: The marked target takes 50% more damage from all melee attacks, (excluding your attacks.) **\[Protection\]**: The marked target takes 50% less damage from damage, as long as you are within 3 sqrs of them. **\[Assassination\]**: The marked target takes 50% more damage from your attacks, as long as they are not targeting you. (They need to have a target in order to get the damage buff), (This only works on hostile mobs) **\[Aid\]**: The marked target heals 4 HP every time you attack a mob. This has a cooldown of half a second. | If the user has other \[Mark\] effects, all of their effects are added to the same ability. |
| Cloaker Fields \[X\] | 200 ahn / 8 EP | You gain a new ability called “Cloak”. When you activate this ability, you will become hard to see, and will gain the “City” faction for 10 seconds. This will end early if you perform a melee attack or start opening crates. |  |
| **Negative Effects** *These are all of the effects which have a negative cost, letting you spend more points at the cost of some downsides.* |  |  |  |
|  |  |  |  |

# New Machine: Attachment Fabricator

*This is a machine that can be found in the Workshop. You can only use it if you have the ID with the correct access. If you pass that check, it opens a similar but simpler UI compared to the augment fabricator.*

*Attachments are small items that can be attached to objects in or above the ‘ego\_weapon’ subtype. Giving that weapon extra effects and downsides. They can also be easily removed by alt-clicking a weapon with an attachment. It takes 5 seconds to attach/remove an attachment.*

## Effects/Flavor

Being similar to the augment fabricator, when you open UI you will see a page. On the top of the page you will be able to change the attachment’s name, description, rank and color. 

Similar to the augments, ranks raise the base EP of the attachment (which is always 4\) where it gets extra EP equal to \[Rank\*2\]. However, at ranks higher than 1\. The attachment will change its attribute requirements to the following (Rank 2: 40, Rank 3: 60, Rank 4: 80, Rank 5: 100). The attachment will check the attribute requirements of the weapon. If the current requirements for an attribute are lower than the requirements caused by the augment, it will change them to a higher value.  
When the attachment is removed, all attribute requirements are reduced to their original amounts. If any were changed.

Then, at the bottom of the page you will be able to pick what effects you are able to add to your attachment. Works the same way it works for the augment fabricator. You add effects as long as you have enough EP points.

Here is the list:

| Effect Name | Ahn / EP cost | Effect Description | Properties |
| :---: | :---: | :---: | :---: |
| Sharpness \+ | 25 ahn / 2 EP | On hit, Inflict 1 Bleed, Doubled if the weapon has an attack speed greater than 1 second.(Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Heated \+ | 25 ahn / 2 EP | On hit, Inflict 1 Burn, Doubled if the weapon has an attack speed greater than 1 second. (Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Quivering \+ | 25 ahn / 2 EP | On hit, Inflict 1 Tremor, Doubled if the weapon has an attack speed greater than 1 second. (Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Splattering | 50 ahn / 4 EP | On hit, inflict 1 bleed to all non-humans within 1 sqr of the target. |  |
| Ink Over | 50 ahn / 4 EP | When attacking a target with 10+ bleed, deal RED damage to the target, equal to the target’s bleed \*2, then reduce the bleed on target by half. This has a cooldown of 4 seconds |  |
| Brand | 50 ahn / 4 EP | When attacking a target with 8+ burn, inflict 1 WHITE Fragility |  |
| Scorching Strike | 50 ahn / 4 EP | When attacking a target with 10+ burn, inflict Damage Down equal to the target’s burn / 4\. This has a cooldown of 6 seconds |  |
| Enduring | 50 ahn / 4 EP | When attacking a target with 8+ tremor, gain 1 RED and BLACK Protection |  |
| Reversal Convulsion | 50 ahn / 4 EP | When attacking a target with 10+ tremor, trigger a tremor burst and give yourself 3 RED and BLACK Protection. Then reduce the target’s tremor by half. This has a cooldown of 4 seconds |  |
| Sharpness \- | 25 ahn / \-2 EP | On hit, Gain 1\*X Bleed, Doubled if the weapon has an attack speed greater than 1 second.(Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Heated \- | 25 ahn / \-2 EP | On hit, Gain 1\*X Burn, Doubled if the weapon has an attack speed greater than 1 second. (Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Quivering \- | 25 ahn / \-2 EP | On hit, Gain 1\*X Tremor, Doubled if the weapon has an attack speed greater than 1 second.(Has a cooldown of half a second) | \[Repeatable, Max of 3\] |
| Heavy Weight | 50 ahn / \-4 EP | Decrease the attack speed of the weapon by 1\*X second. | \[Repeatable, Max of 2\] |

# 

