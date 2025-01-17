+++
date = '2025-01-17T15:29:53-07:00'
draft = false
title = 'Test'

+++


Kaboom Arena

# Core Game Loop

- Team Death Match
- All teammate damage is enabled (friendly fire).

# Combat

## Main Input

- **Left Mouse**: [Tossing](app://obsidian.md/index.html#tossing)
- **Right Mouse**: [Interaction](app://obsidian.md/index.html#interaction)

## Grenade

### Grenade Definition

- Players must pick up grenades from [Grenade Pickup](app://obsidian.md/index.html#grenade pickup) locations on the map.
- Each toss consumes one grenade from the player's [Inventory](app://obsidian.md/index.html#inventory).

### Grenade Damage

- **Direct Hit**: Instant kill.
- **Area of Effect (AOE)**: Damage decreases with distance from the explosion center.

### Special Grenades

Special grenades apply unique effects in addition to the base grenade damage.

Examples:

1. **Molotov**: Creates a persistent damage area.
2. **Ice Orb**: Slows players in the affected area.
3. **HE (High-Explosive)**: Large damage radius with high damage.
4. **Knockback Grenade**: Adds an impulse force to impacted players.
5. **Healing Grenade**: No damage. Direct hits restore full health. Creates a healing area.
6. **Mine**: Remains on the ground and triggers when stepped on.

### Grenade Pickup

- **Grenade Pickup Objects** spawn randomly across the map.
- Different types of grenades have different spawn probabilities.

## Tossing

- Press and hold **Left Mouse** to display a projectile trajectory indicator.
- Release **Left Mouse** to toss the grenade along the indicated trajectory.
- A short cooldown is required between each toss.

## Interaction

- Hold **Right Mouse** to interact with environmental objects.
- Interactions require a specific amount of time to complete.

### Example Interaction

- Pick up: Interact with **Grenade Pickup Objects** to add the corresponding grenade to your [Inventory](app://obsidian.md/index.html#inventory).

## Inventory

- Players can hold a maximum of **3 grenades** at a time, regardless of type.
- A **quick bar UI** displays the current grenade reserve.
- Players can switch grenade types using a designated input.

# Ability

- Abilities focus on non-damage and movement-related effects.
- Each character has a distinct set of abilities.

## Example Ability List

1. **Dash**: Quickly move in the direction the player is facing.
2. **Ice Wall**: Create a temporary blocking wall.
3. **Blind**: Obscure the vision of enemies in front of the player.
4. **Shield**: Block one instance of damage.
5. **Sprint**: Temporarily increase movement speed.
6. **Invincible**: Become immune to damage for a short period, but unable to move or attack.

# Level Design

- Levels should include multiple high-ground areas that players can climb to for strategic advantage.

# Future Plan

## In-Game Progress

- As the game progresses, players earn **resources** (XP or currency).
- Players use these resources to enhance their [Attributes](app://obsidian.md/index.html#attribute) or acquire [Roguelike Cards](app://obsidian.md/index.html#roguelike card)

## Attribute

Attributes improve various aspects of the player character. Different attributes have unique effects.

Examples:

1. **Increased Grenade Capacity**: Allows the player to hold more grenades.
2. **Enhanced Movement Speed**: Boosts the player’s base speed.
3. **Cooldown** **Reduction**: Shortens the cooldowns for abilities and grenade tosses.

## Roguelike Card

- Abilities are decoupled from characters and acquired through **cards**.
- Players can hold a maximum of **4 cards** at a time.
- Cards are activated using the **1-4** keys, with some providing passive effects or buffs.
- **Card Acquisition**: Players obtain cards through a lottery system, introducing a roguelike element similar to games like *Balatro*.
