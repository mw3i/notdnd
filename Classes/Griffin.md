---
title: Griffin
trait: range
environment: metal
---

![Source: LynxKano @ https://www.deviantart.com/lynxkano/art/dodging-333329314](../assets/griffin-class.jpg){: width="40%"}

- health: 30
- weapon: [**The Crane's Wing**](../Weapons)
    - made of metal; requires user to wear a metal band around palm
    - can be thrown up to 4 dashes

<!-- 
  - requires 2 dodges to avoid if target is 2-3 paces away
-->


# Spells

## Lvl 1: "ar-sink" (Push/Pull)
```yaml
roll: . (1d6 for damage calc)
recharge: 1 turn
```

Push or pull objects 

- targeting distance: 6 dashes / mass 
- push/pull distance:
    - small obj: 6 spaces
    - med obj: 3 spaces
    - large obj: 1 space
- if used as a damage attack
    - damage = roll / obj mass

> Masses:
> - light obj = 1 (e.g., a rock)
> - medium obj = 2 (e.g., human)
> - heavy obj = 6 (e.g., massive boulder)
> 
> Based on the Force = Mass * Acceleration equation where:
> - Force <=> Roll
> - Acceleration <=> Damage  	
> (don't know if that makes sense but good enough)


<!-- medium objects add +2 if throwing downwards; heavy objects: add +4 if throwing downwards -->

<!-- 
Secret move unlocks:
- can extend the boomerang
- can propel self in the air 3 spaces (by pushing off the ground)
- can hit two people at once
- can be used on same person (have to roll for each one
- ^ double hits have to follow a reasonable boomerang shape
 -->

## Lvl 2: "echo" (Mirror Portal)
```yaml
roll: 1d8
recharge: 3 turns
```

Cast a portal at any location within 2 dashes. Stays where it's at till the start of your _next_ turn. 

<!-- boomerang can be thrown around it -->

- roll <= 4: absorbs any physical or spell based attack
- roll >= 4: damage reflected back at attack (who either takes the damage or has to use a dodge to escape).
    - amount of damage reflected depends on the damage from the attacker's roll

Can be cast as a reaction.

> [!World]
> The timing of the "absorb" and "reflect" aspects of the mirror are staggered 1 action unit in time. Otherwise, reflecting matter back would just cause something to collide into itself and do nothing.

Also: the portal is 1 directional; that is, if you throw something from behind the portal, it just moves through it as it normally would.

<!-- secret move: cast a portal below yourself and jump in it; can be used as counter that is always successful -->

<!-- 
## Lvl 3 (special): "ex-lynk" (Current)

```yaml
roll: 1d20 >>
charge: 1 turn
recharge: 1 day
```

Throw the boomerang in a large cone (w/ length of 5 dashes). Everyone in the cone (including teammates):

- takes damage equal to the dice rollover
- are stunned

> cuz they're stunned by the electrocution

nat 20: get an extra boomerang throw before your turn ends 
-->