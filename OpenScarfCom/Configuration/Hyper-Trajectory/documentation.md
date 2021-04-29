# Basics of trajectories.rul

_trajectories.rul_ consists of three parts:

- Colors
- Refnode Vapor
- Weapon Vapor

each part heavily uses _refNode_ function.

## Colors

a typical color refnode:

    - &COLOR_WHITE # Name to be referenced
      type: COLOR_WHITE
      vaporColorSurface: 0 # index in _transparency.rul_

All _colors_ are refNodes, so it can be referenced by _Refnode Vapor_.

## Refnode Vapor

a typical refnode vapor:

    - &VAPOR_ROCKET_CLASS_D # Name to be referenced
      type: VAPOR_ROCKET_CLASS_D
      refNode: *COLOR_WHITE # Color value it is referencing
      vaporDensity: 80 # Underwater Missions
      vaporDensitySurface: 100 # Surface Missions
      (optional) vaporProbabilitySurface: 15 # default 15

All _ref vapors_ are refNodes, so it can be referenced by _Weapon Vapor_.

## Weapon Vapor

a typical weapon vapor:

    - type: STR_LARGE_ROCKET
      refNode: *VAPOR_ROCKET_CLASS_D

Choose any _Refnode Vapor_ of your choice (or make one) then reference it with refnode. Vapors should be defined on either

- ammos
- internal ammo weapons (lasers, terror unit weapons, etc)

It is recommended to only add vapor related flags to _trajectories.rul_ for better visibility.

---

# Basics of hypervelocity.rul

_hypervelocity.rul_ consists of two parts:

- Presets
- Weapon Speed

each part heavily uses _refNode_ function.

## Presets

### Global

    - &VELOCITY_GLOBAL # Name to be referenced
      type: HYPERVELOCITY_GLOBAL
      confAuto:
        followProjectiles: false # does not follow bullets when firing auto
      explosionSpeed: 2 # 200% explosion/bullet hit animation speed
      bulletSpeed: 20 # How fast a bullet moves, 0 vanilla default, 20 vanilla max

Every presets are referenced by _global_.

### Root Preset

a typical _root_ preset:

    - &VELOCITY_BALLISTIC # Name to be referenced
      type: VELOCITY_BALLISTIC
      refNode: *VELOCITY_GLOBAL # References Global
      explosionSpeed: 2

Each branch of weapon types are referenced by _root_ presets.

### Preset

a typical preset:

    - &VELOCITY_BALLISTIC_LO # Name to be referenced
      type: VELOCITY_BALLISTIC_LO
      refNode: *VELOCITY_BALLISTIC # References its root node
      (optional) bulletSpeed: 20
      (optional) explosionSpeed: 3

## Weapon Speed

a typical weapon speed:

    - type: STR_HC_AP_AMMO
      refNode: *VELOCITY_BALLISTIC_LO
      explosionSpeed: 3
      (others...)

It is recommended to only add velocity and animation speed related flags to _hypervelocity.rul_ for better visibility.
