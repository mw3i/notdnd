---
title: Not DnD
color-links: true
version: 0.1
---

<!-- Links: [Weapons](Weapons.md) | [Dragon Class](Classes/Dragon.md) | [Griffin Class](Classes/Griffin.md) | [Hydra Class](Classes/Hydra.md) -->

The purpose of the game is to advance the story by exploring the world. You win when the story ends.

**Required Die**: 1d4, 1d6, 1d20

# Combat

For each round, for each player, perform 3 actions in any order:

| Action           | Effect                       | roll      |
| -                | -                            | -         |
| do nothing       | <--                          |           |
| dash (ced)       | move 1 dash (tile)           |           |
| punch            | 1 damage                     |           |
| weapon           | up to 4 damage (use roll)    | 2+ on 1d4 |
| cast base spell  | see [base spells]            |           |
| cast lvl 1 spell | see [class]; 1 turn recharge | 3+ on 1d6 |

<!-- | cast spell 2    | see [class]; 3 turn recharge | 3+ on 1d6   | -->
<!-- | cast special    | see [class]; 1 day recharge  | 6+ on 1d20  | -->
<!-- | cast ultimate   | 1 per campaign             | always land | -->

If you haven't used all 3 actions yet, you can do the following outside of your turn:

| ReAction | Effect                                                   | roll |
| -        | -                                                        | -    |
| dodge    | move 1 dash away from target; don't take damage          |      |
| counter  | roll against opponent; higher roll means attack is yours |      |
| cast     | some spells can be case as reactions                     |      |

If an an action roll fails to meet threshold, recharge doesn't go into effect. 

<details>
<summary>^ Rationale</summary>
Caster is already penalized if they fail to meet roll threshold: they wasted an action.

This also ensures more spells get used; you're more likely to risk using a spell if you know that you can just keep trying with more actions. Ie, if a caster really wants to use a spell, they're gunna eventually land it

Allows for more fluid strategy planning because your entire plan doesn't get frequently steamrolled by a bad roll.

If the spell was successful, but the opponents dodge -- that still triggers a recharge (just means you missed)
</details>

## Conflict Logic

1. Attacker declares action
2. Defender (if any) declares response (dodge, defend)
    - IF **dodge**: no damage (if you can dodge to an area outside the range of effect; can chain dodges if necessary)
    - IF **counter**: roll the same dice as attacker; if higher: you get to deal weapon damage instead
<!--     - IF **block**: roll against opponents die; opp roll - your roll = damage dealt. -->
<!--     - If negative, deal damage to attacker (i.e., a _counter_) -->


<!-- <details>
<summary>^ Rationale</summary>
I'm a fan of this new logic system because it makes the "tandem roll" feel like an actual competition to roll high. It doesn't solve the gridlock issue (requiring attacker to wait for opponent to decide before round progression), it at least makes things "memory-less" (rolls are calculated _after_ action and reaction are both declared). We might have to change the roll threshold for dodging if I end up removing roll thresholds all together (maybe like, half your opponents roll round up).

This allow allows adding dice modifiers; like, if you use "burst", your modifier would carry into the roll of whatever next action you use.

This also gives advantage to the attacker, which seems fair. The attacker can still take damage if countered, but it's not as drastic.
</details>
 -->
---

# Base Spells

| spell | description                                                  | combat effect                         |
| -     | -                                                            | -                                     |
| los   | magic vision; reveals information about the world around you | cut roll threshold in half (round up) |
| ced   | jump quickly in super-human strides                          | world mechanic for dash and dodge     |
| rom   | blast a burst of energy out of your hands                    | roll +2 on 1d4 w/ damage rollover     |





