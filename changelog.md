## 2021.04.30 - v0.1.6a "Takt1kz Impr0v3d"

### modified

- alien deployment numbers fixed to beginner default
  - also any opinions welcome; does this make game _fun_ or it doesn't?

## 2021.04.29 - v0.1.5a "Ammo Day 3"

### added

- new sprite for rocket launcher

### modified

- rocket launcher blind shot firing mode added; low tu cost but almost zero accuracy

- incendiary rounds changed to thermobaric rounds

  - power is _literal_ now; deals heavy incendiary damage
  - can break through one or two brick walls
  - one-shots sectoids and floaters
  - more costly and slightly less powerful than HE equivalent
  - TODO: make rounds tagged as thermobaric deal small damage to units immune to incendiary too

- aliens does not carry primed grenades anymore

  - because it might discourage players from fighting inside UFO
  - opinions are welcome (a: revert, b: keep it, c: make it random, etc)

- refactored alien deployment and missions

## 2021.04.28 - v0.1.4a "Ammo Day 2"

### added

- magazines now show different sprites for ammos left
  - currently for Heavy Cannon ammo

### modified

- several assets rearrangements
- scripts refactored to be more intuitive
  - changed local variable styles to be distinctive from API variables

## 2021.04.27 - v0.1.3a "Ammo Day"

### added

- weapons can now show different sprites up to 4 based on loaded ammo

  - total 16 possible combinations (for (possible) modders)

- new weapon: automatic rifle/grenade launcher
  - uses same ammo with heavy cannon
  - currently wip: seriously OP because all 6 HC clips are loaded at once; will make a feature to compensate this asap
  - use at your own risk!

### modified

- sprite assets for weapons with different sprites based on different ammo renamed to be more intuitive

## 2021.04.26 - v0.1.2a "Air Day"

### added

- Hunter Killers

  - ufos have around 20 ~ 40% chance to spawn as hunter killers
  - hunter killers have 50% spawn chance to escape when damaged
  - HK would target interceptors first, but could also target transport craft if alone
    - which is the reason skyranger got built-in cannon
  - repair rate **fivefolded** to compensate the HK threat

- new grenade looks for smoke and frag

- automatic rifle color brightened to match up more with other ballistic tier weapons

### modified

aircraft weapons buff: they were so useless before; now it would stand more chance against ufos and prove some usefulness. to balance, maybe increase cost? to compensate with overall easier dogfight, ufos will also have its buffs, to be added someday...

- missile specs buffed

  - projectile speed **doubled**
  - stingray rate of fire **increased**: **[64, 48, 32] -> [48, 32, 20]**
  - ammo **increased**:
    - avalanche: **3 -> 4**
    - fusion ball: **2 -> 4**

- cannon specs buffed (would come handy for future hunter-killer implementations)

  - damage, rate of fire, firing range, projectile speed **doubled**
  - **_no ammo_ needed**: no chores, more fun!
  - now interceptor and skyranger **built-in weapon** (your fightor has **3 weapons pod** total)

- laser cannon buffed

  - range **doubled** (42, the answer to life, universe, and everything)

- arranged armors and weapons into subdirectories (took more time then it seems)

### bugfixes

- annoying error that says `laser tank not on manufacture`
- spritesheet load error (don't use `singlefile` on _spritesheet_))
- also various ones with rifles

## 2021.04.25 - v0.1.0a

- initial release
