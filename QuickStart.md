---
title: Not DnD
color-links: true
version: 0.1
---

<!-- Links: [Weapons](Weapons.md) | [Dragon Class](Classes/Dragon.md) | [Griffin Class](Classes/Griffin.md) | [Hydra Class](Classes/Hydra.md) -->

The purpose of the game is to advance the story by exploring the world. You win when the story ends.

**Required Die**: 1d4, 1d6, 1d8, 1d20

# Combat

## Actions

For each round, for each player, perform 3 actions in any order:

| Action           | Effect                       | roll |
| -                | -                            | -    |
| do nothing       | <--                          |      |
| dash (ced)       | move 1 dash (tile)           |      |
| punch            | 1 damage                     |      |
| weapon           | up to 4 damage (use roll)    | 1d4  |
| cast base spell  | see [base spells]            |      |
| cast lvl 1 spell | see [class]; 1 turn recharge | 1d6  |
| cast lvl 2 spell | see [class]; 2 turn recharge | 1d8  |


<!-- | cast special    | see [class]; 1 encounter recharge; 3 charge actions required | 6+ on 1d20  | -->
<!-- | cast ultimate   | 1 per campaign             | always land | -->

## Reactions

If you haven't used all 3 actions yet, you can do the following outside of your turn:

| ReAction | Effect                                                   | roll |
| -        | -                                                        | -    |
| dodge    | move 1 dash away from target; don't take damage          |      |
| counter  | roll against opponent; higher roll means attack is yours |      |
| cast     | some spells can be case as reactions                     |      |

## Team Chaining

<details>
<summary>If it's your turn, you can let a teammate expend an action in your stead. You don't lose the action, but you dont get to use it on your turn.</summary>
This mechanic allows team-action combos with a reasonable limitation, and avoids the problem of race conditions if the gameplay was 100% asynchronous. 

It's intentionally not: "give away as many actions you have left" <-- otherwise a player could just give away their whole turn to the rest of the team, which seems kinda dumb.

One downside: this by itself doesn't allow 3 person chaining, which would be cool (though that can still happen via other reaction mechanics). Could fix that with "give away up to 2 actions, but only 1 action per teammate" but for now let's see how the 1 action limit goes.
</details>


## Conflict Logic



1. Attacker declares action
2. Defender (if any) declares response (dodge, defend)
    - IF **dodge**: no damage (if you can dodge to an area outside the range of effect; can chain dodges if necessary)
    - IF **counter**: roll the dice of your counter weapon / spell; if higher: you get to deal damage instead (not all spells can be used as counters)

<!-- 
Alt Version
1. Attacker declares action
2. Attacker rolls action dice; Defender rolls Shield dice
    - IF defender rolls higher: counter damage with your roll - their roll
    - IF attacker rolls higher: take damage 
Could even do: dodge costs 2 actions
-->


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

| spell | description                                                  | combat effect                                                            |
| -     | -                                                            | -                                                                        |
| los   | magic vision; reveals information about the world around you | weapon attacks are undodgeable (amybe this is the mechanic for dodging?) |
| ced   | jump quickly in super-human strides                          | nothing; it's just the world mechanic for dash and dodge                 |
| rom   | blast a burst of energy out of your hands                    | 1d4 attack                                                               |







