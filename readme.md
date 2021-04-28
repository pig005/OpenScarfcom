# OpenScarfCom

**Total Conversion Mod** focused on **replayability** for **OpenXcom Extended**

being developped by _greenscarf_ (for now) and released under [gpl v3.0](./OpenScarfCom/LICENSE) [(\*)](#submod-credits)

please report any bugs/ideas on `issues`.

## CHANGELOGS

check [**changelog.md**](./changelog.md) for more details

## PRECAUTIONS

OpenScarfCom (OSC for short) is under alpha phase of development; it could be filled with

- Unknown fatal bugs
- Seriously unbalanced aspects
- Unplanned behaviors

it is recommended to

- Not turn on IRONMAN (due to possible bugs corrupting saves)
- Use Debug mode (ctrl + D, can be turned on in options.cfg)
- Backup your game data

## HOW TO INSTALL

OSC needs latest [OXCE](https://openxcom.mod.io/openxcom-extended "link to OXCE mod.io page") to run properly.

1. download OSC on [mod.io](https://openxcom.mod.io/openscarfcom "link to OSC mod.io page")(relatively bug-free) or cloning the repository (nightly, bug-prone)
2. move the repository to My `PC/Documents/OpenXcom/mods`
3. run **latest** OXCE then press `mods`
4. enable OpenScarfCom

## PLANNED FEATURES / DONE

there is one design philosophy for OpenScarfCom: make it more replayable.

([V]: done / [ ]: wip / everything else: **LONG TERM GOAL**)

- **Quality Of Life** features

  - [x] All crafts now **auto-patrol**
  - [x] [Hyper & Trajectory](https://openxcom.mod.io/oxce-hyper-velocity1) integrated
  - [x] Destroy alien base to make countries reconsider their pact with aliens and join X-COM project again
  - [x] Different sprites for loaded/unloaded weapons
  - [x] Different sprites for magazines by ammos left
  - [ ] Reduce real-time spent on `Research` and `Manufacture` (priority)
    - [ ] One item, multiple variations
  - [ ] Easier item and units overhauls and upgrades
  - better fund mechanics
    - disable making profit with manufacture
    - huge score-driven fund bonuses

- Improved **Alien AI**
  - [x] Spotter & Sniper tactics
  - [x] Carry multiple pre-primed grenades
  - Melee attack for all & pick up weapons
  - Change tactics depending on situations
- Enhanced **Tactical Combat**
  - [x] Using environment for advantage
    - smoke stun damage increased
      - aliens can now be stunned by smokes
    - fire is now **lethal**
      - fire damage threefolded
      - standing on fire can inflict up to 20 fatal wounds
  - fatal wounds reduces morale
    - units with high bravery will negate most of the morale loss
  - [x] Medikit can be used alone and recovers more energy
  - [ ] Sniper weapons have aimed shot as reaction fire
  - [ ] Automatic firearms have auto shot as reaction fire
  - [ ] More randomness (maps, enemy loadouts, etc../)
  - [ ] One feature, multiple uses (laser weapons can switch to 'shotgun' mod, plasma 'overcharge', etc)
  - Directional lightings and visions
- Enhanced **Aerial Combat**
  - [ ] hunter-killer ufos (can also retreat)
  - retaliation terror ship (can be either armed with missile or boarding troop)
  - make all weapons viable (apart from avalanche and plasma beam spam)
    - [x] double missile projectile speed (hit satisfaction)
    - [x] buff fusion ball launcher
  - ufo shields and nukes to counter them
  - more meaningful interactions (other than careful/aggressive)
    - [x] built-in cannons for interceptor and skyranger
- **Replayability**
  - [ ] Balancing based on **IRONMAN** playthrough
  - Alien strategy changes based on your actions
  - Story arcs
  - Multi endings
  - Make every mission meaningful (even failed ones)
  - Overall same or less playtime than vanilla X-COM
- the **OSC** itself
  - [x] Conventional Commits
  - [x] Directory Organization
  - [ ] Automated changelog generation
  - Automated release generation
  - Ruleset/Scripting Conventions
  - Detailed Documentations
  - Transifex support
  - Automatic uploads to mod.io after pushes

## HOW TO CONTRIBUTE

you could always do a pull request! if it suits the design philosopy above, it will be merged as soon as possible. if not, we could always discuss to make possible modifications.

## SUBMOD CREDITS

the [gpl license](./OpenScarfCom/LICENSE) only applies to `OpenScarfCom` directry. other folders are unaffected by this license. also if you're not satisfied with the license i could send you CC0-licensed codes that I wrote.

> i have no rights to any of the mods included below.

scarfcom could not have been developed without help from these mods. mod assets are in seperate folders. these mods included are out of my bounds all rights goes to their respective owners.

if you are the author of these mods and do not wish these mods to be used, please let me know, or PM me on openxcom forums, or contact me with `honestlawn005@gmail.com.` **it will be removed immediately**.

included mods:

- [**Community Map Pack**](https://openxcom.mod.io/community-map-pack)
  by CMP admin and various contributers, licenced under CC-BY-NC
- [**Extra Explosions**](https://openxcom.mod.io/extra-explosions)
  by Arathanor, Strarvingpoet
- [**AWACS AIRCRAFT**](https://openxcom.org/forum/index.php?topic=2952)
  by redv
- [**HQ sounds**](https://openxcom.mod.io/hqsounds-by-daedalus)
  by daedalus, hellrazor
- [**Combat Armor**](https://openxcom.org/forum/index.php?topic=1281)
  by Warboy1982, Ryskeliini
  recolor by Solarius Scorch
