---
hidden: true
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Конфигурация сервера

Здесь вы можете ознакомиться с конфигурацией сервера, если вы конечно знаете, что и за что должно отвечать.

**Процессор:** три ядра R9-9950X

**ОЗУ:** 12ГБ DDr5

**Ядро:** LeafMC 1.21.8

## `server.proporties`

```
difficulty=hard
simulation-distance=7
view-distance=8
```

## `bukkit.yml`

```
spawn-limits:
  monsters: 49
  animals: 7
  water-animals: 5
  water-ambient: 14
  water-underground-creature: 5
  axolotls: 5
  ambient: 5
chunk-gc:
  period-in-ticks: 400
ticks-per:
  animal-spawns: 400
  monster-spawns: 4
  water-spawns: 200
  water-ambient-spawns: 200
  water-underground-creature-spawns: 200
  axolotl-spawns: 200
  ambient-spawns: 200
  autosave: 6000
```

## `spigot.yml`

```
world-settings:
  default:
    view-distance: default
    simulation-distance: default
    thunder-chance: 100000
    merge-radius:
      item: 0.5
      exp: -1.0
    mob-spawn-range: 7
    item-despawn-rate: 6000
    arrow-despawn-rate: 1200
    trident-despawn-rate: 1200
    zombie-aggressive-towards-villager: true
    nerf-spawner-mobs: false
    enable-zombie-pigmen-portal-spawns: true
    wither-spawn-sound-radius: 0
    end-portal-sound-radius: 0
    hanging-tick-frequency: 100
    unload-frozen-chunks: false
    growth:
      cactus-modifier: 100
      cane-modifier: 100
      melon-modifier: 100
      mushroom-modifier: 100
      pumpkin-modifier: 100
      sapling-modifier: 100
      beetroot-modifier: 100
      carrot-modifier: 100
      potato-modifier: 100
      torchflower-modifier: 100
      wheat-modifier: 100
      netherwart-modifier: 100
      vine-modifier: 100
      cocoa-modifier: 100
      bamboo-modifier: 100
      sweetberry-modifier: 100
      kelp-modifier: 100
      twistingvines-modifier: 100
      weepingvines-modifier: 100
      cavevines-modifier: 100
      glowberry-modifier: 100
      pitcherplant-modifier: 100
    entity-activation-range:
      animals: 24
      monsters: 32
      raiders: 48
      misc: 16
      water: 16
      villagers: 24
      flying-monsters: 32
      wake-up-inactive:
        animals-max-per-tick: 4
        animals-every: 1200
        animals-for: 100
        monsters-max-per-tick: 8
        monsters-every: 400
        monsters-for: 100
        villagers-max-per-tick: 4
        villagers-every: 600
        villagers-for: 100
        flying-monsters-max-per-tick: 8
        flying-monsters-every: 200
        flying-monsters-for: 100
      villagers-work-immunity-after: 100
      villagers-work-immunity-for: 20
      villagers-active-for-panic: true
      tick-inactive-villagers: true
      ignore-spectators: false
    entity-tracking-range:
      players: 96
      animals: 80
      monsters: 80
      misc: 80
      display: 96
      other: 64
    ticks-per:
      hopper-transfer: 8
      hopper-check: 1
    hopper-amount: 1
    hopper-can-load-chunks: false
    dragon-death-sound-radius: 0
    hunger:
      jump-walk-exhaustion: 0.05
      jump-sprint-exhaustion: 0.2
      combat-exhaustion: 0.1
      regen-exhaustion: 6.0
      swim-multiplier: 0.01
      sprint-multiplier: 0.1
      other-multiplier: 0.0
    max-tnt-per-tick: 100
    max-tick-time:
      tile: 50
      entity: 50
```

## `config\paper-global.yml`

```
unsupported-settings:
  allow-headless-pistons: false
  allow-permanent-block-break-exploits: true
  allow-piston-duplication: false
  allow-unsafe-end-portal-teleportation: false
```

## `config\paper-world-defaults.yml`

```
  behavior:
    allow-spider-world-border-climbing: true
    baby-zombie-movement-modifier: 0.5
    cooldown-failed-beehive-releases: true
    disable-chest-cat-detection: false
    disable-creeper-lingering-effect: false
    disable-player-crits: false
    door-breaking-difficulty:
      husk:
      - HARD
      vindicator:
      - NORMAL
      - HARD
      zombie:
      - HARD
      zombie_villager:
      - HARD
      zombified_piglin:
      - HARD
    ender-dragons-death-always-places-dragon-egg: false
    experience-merge-max-value: -1
    mobs-can-always-pick-up-loot:
      skeletons: false
      zombies: false
    nerf-pigmen-from-nether-portals: false
    only-merge-items-horizontally: false
    parrots-are-unaffected-by-player-movement: false
    phantoms-do-not-spawn-on-creative-players: true
    phantoms-only-attack-insomniacs: true
    phantoms-spawn-attempt-max-seconds: 119
    phantoms-spawn-attempt-min-seconds: 60
    piglins-guard-chests: true
    pillager-patrols:
      disable: false
      spawn-chance: 0.2
      spawn-delay:
        per-player: false
        ticks: 12000
      start:
        day: 5
        per-player: false
    player-insomnia-start-ticks: 72000
    should-remove-dragon: false
    spawner-nerfed-mobs-should-jump: false
    stuck-entity-poi-retry-delay: 200
    zombie-villager-infection-chance: default
    zombies-target-turtle-eggs: true
  spawning:
    despawn-range-shape: ELLIPSOID
    despawn-ranges:
      ambient:
        hard: default
        soft: default
      axolotls:
        hard: default
        soft: default
      creature:
        hard: default
        soft: default
      misc:
        hard: default
        soft: default
      monster:
        hard: default
        soft: default
      underground_water_creature:
        hard: default
        soft: default
      water_ambient:
        hard: default
        soft: default
      water_creature:
        hard: default
        soft: default
    despawn-time:
      llama_spit: disabled
      snowball: disabled
```

## `config\leaf-global.yml`

```
performance:
  dab:
    enabled: true
    dont-enable-if-in-water: false
    start-distance: 16
    max-tick-freq: 20
    activation-dist-mod: 9
    blacklisted-entities:
    - villager
    - axolotl
    - hoglin
    - zombified_piglin
    - goat
```
