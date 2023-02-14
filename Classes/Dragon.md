---
title: Dragon
trait: power
environment: stone
---

health: 25
weapon: **Dragon's Claw** (Lance)
- made of wood and metal
- +2 on all attacks


# Spells

## Lvl 1: Burst-Mode
```yaml
roll: 3+ on 1d6 >>
recharge: 1 turn
```

Adds buffs to other actions; choose:

- , x3 distance on a single dash (but can only be in one direction; cant change angles)
- rom: add damage to rom attack; push back 3 spaces
- weapon: add roll to attack (flavoring: takes two swings with lance)

Rules:
- only works on self

<!-- originally i wanted the land threshold to increase to represent the user flailing and failing because of the extra power that's harder to control; but we already kinda get that with the init threshold, so might as well just make it a flavoring when the event actually happens than trying to build it in mechanically-->
<!-- 
## Lvl 2: Fire
```yaml
roll: 3+ on 1d6 >> x2
recharge: 3 turns
range: 4 paces
```

Breath a powerful stream fire towards anyone within 2 dashes

> think: cyclops from x-men, but with fire

- damage rollover can be spread across opponents
- drop as many "fire tiles" as you have rolls
    - each one deals +2 damage if stepped on
    - each tile has to be adjacent to the last
    - tiles last 2 rounds


## Lvl 3 (special): Guts-Mode
```yaml
roll: 6+ on 1d20 >>
charge: 1 turn
recharge: 1 day
```
[6+ on 1d20; 1 day recharge]

Recharge all spells

Then: Perform 10 actions in a row.

Rules:

- can only be used when health is 5 or fewer
- can be used in response to getting attacked (if resulting is health is 5 or fewer)

Nat 20: +2 actions (so, 12 total) -->