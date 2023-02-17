---
title: Rule Book
color-links: true
---


# Overview

The purpose of the game is to advance the story by exploring the world. You win when the story ends.

**Required Dice**:

- [ ] 1d4
- [ ] 1d6
- [ ] 1d20


# Characters

- Pick a class
	- [dragon (red) style](Classes/Dragon.md)
	- [crane (blue) style](Classes/Crane.md)
	- [snake (green) style](Classes/Snake.md)

> There are other classes but you don't get to pick them.


# Combat

Asyc Turn-based

- i.e., you can do shit on other people's turn, sometimes

On each turn, you get 3 actions; pick any combination of:

- Dash
- Strike (Punch, Weapon)
- Cast Spell
- React (Dodge, Counter, React Spell)
- Do Nothing

Why would you do nothing? 

> **Action Rollover**: If you have remaining action slots, they can be utilized on someone (or something) else's turn.
> 
> ^ this pressures you into deciding whether you want to save a spell for a dodge or use all your spells at once; this will vary by player type and scenario.
> 
> ^ it also makes the combat "async" turn based.

Some actions require a roll threshold. 

- i.e., "2+ on 1d4" means you need to roll 2 or higher on a d4 for the action to be successful

> **Damage Rollover**: If a threshold for a damage action is reached, the number rolled is the damage dealt.

## Actions

### Dash

"Dashing" is moving in a short, fast burst in some direction.

Dashes are used as the primary metric of distance. 

- e.g., player X might be "2 dashes" away from player Y

> [!World]
> Performing a dash is actually casting the "ced" spell. If you lose the ability to cast any magic, you cannot dash.


### Strike

Physically strike an opponent with your fists or a weapon.

- Punch: 1 damage
- Weapon: 2+ on 1d4 w/ damage rollover

<!-- 
#### Dash Attack

If adjacent to an opponent, spend 2 moves to dash into the opponents tile, and make an attack.

- can't be dodged
- opponent moves 1 tile backwards (in direction of your dash)

Removing this with the change of 
 -->

### Spell Casting

Magic drains chakra. Chakra recharges (faster in sunlight).

> - Charge: Time it takes to cast
>	- interrupted if the user takes damage (swatted)
>	- a user charging can't attack but can dodge
> - Recharge: Time it takes to cast again

You can only cast 1 spell at a time.

> Casting a spell requires "shouting" loud enough that your own ears hear your own spell (except for base spells).


#### Base Spells

- Everyone gets them.
- Negligable chakra usage (no charge / recharge)
- Always land; no _roll threshold_ (except _rom_)


#### Advanced Spells (Class-Specific)

Each class gets their own set of advanced spells.

> Class spells require shouting your class + "style" before the spell name. 
> - I.e., "Dragon-style: Rom Star!"

- **Level 1 Spells** [2+ on 1d6]
	- 1 turn recharge

<!-- - **Level 2 Spells** [3+ on 1d6]
	- 3 turn recharge
	- x2 damage rollover -->

<!-- - **Level 3 Spells (Special Attacks)** [6+ on 1d20]
	- 1 turn charge
	- 1 day recharge
 -->

Damage spells get [Damage Rollover].

> All classes have to follow those spell casting rules (though each class spell gets unique effects)

## Reactions

If you have remaining action slots during someone else's turn, you can perform a reactive action.

You can't use a reactive action to attack, unless

- it follows a successful counter
- you are chaining with an active (current turn) player's action

The event logic for reactions are:

- Opponent declares action (e.g., attack)
- You declare rebuttal (e.g., counter)
- You and Opponent roll for success
	- **attacker**: roll above action threshold
	- **defender**: 
		- _dodge_: roll >= Opp's action threshold (e.g., 3+ on a d6 for a lvl 1 spell)
		- _counter_: roll >= Opp's roll

<details>
<summary>Comment</summary>
I'm a fan of this new logic system because it makes the "tandem roll" feel like an actual competition to roll high. It doesn't solve the issue of the gridlock issue (requiring attacker to wait for opponent to decide), it at least makes the event sequence "memory-less" (rolls are calculated _after_ action and reaction are both declared). We might have to change the roll threshold for dodging if I end up removing roll thresholds all together (maybe like, half your opponents roll round up).

This allow allows adding dice modifiers; like, if you use "burst" 
</details>

### Dodge

If you're under attack, you can dodge the attack as many times as you have available slots.

- unless you are stunned

More rules:

- You can dodge if being attacked from behind (backstabbed)
- have to move to a tile non-adjacent from your opponent
- If moving to a non-adjacent tile still leaves you in a moves area-of-effect, you can't technically dodge the move

#### Block

Some weapons allow for "blocking". A block is treated as a dodge, except the user (defender) stays on their current tile

### Counter

Instead of dodging, you can bank on an opponent failing their attack throw. If they fail, you get to respond with an attack.

- You move to a tile adjacent to opponent (if no tiles exist, you can't counter)
<!-- - They can dodge/counter a counter (atm) -->

> Q. Why wouldn't I always counter?
> A. Because you miss the chance to dodge

> A counter is actually a call of the `los` spell

### Cast

Some spells are allowed to be cast as reactions; you can cast those off-turn.


## Damage Calculation
- Damage calculation occurs after a damage action
- Multiplier buffs get applied before Addition buffs


## Statuses
- If **Stunned**:
	-  requires 1 action to recover
	-  can't recover unless it's your turn
	-  cannot perform a reactive action (including dodge)
- If **Downed** (1 health):
	- you can crawl
- If **Knocked out** (1 health and someone does a finishing blow): 
	- you can do nothing until the next day
	- and your team has to haul your ass around


### Death

When you lose all your health, you get knocked out. This doesn't kill you. It's actually very hard to die; it can only happen if:

- you get knocked out and dismembered
- you get vaporized
- you run out of all chakra and chakra reserve.

<!-- make it comically hard die; like just brutally beating up people who are knocked out -->

> Why is it hard to die?
> Humans' (and monsters') bodies are embedded with magic; it allows them to heal from even the most serious of wounds and injuries. When the body is injured, chakra is routed towards healing (and away from normal bodily functions); this causes you to pass out. If you use up all your chakra and your [[chakra reserve]] (a large store of chakra typically inaccessible for spells), you die.


## Recovery
- Short rest: 
	- lvl 1-2 spells recharged
	- gain half of missing health back
- Long rest (1 day):
	- all spells recharged (including special)
	- health set to max
