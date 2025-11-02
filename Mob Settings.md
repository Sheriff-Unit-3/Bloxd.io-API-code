# Mob Settings

These impact the behaviour of mobs, what they look like, and how they sound. These can either be set on a per-mob basis or the default can be set for all mobs of a particular type.

## API Methods to Get/Set Mob Settings
These API methods allow you to modify mob settings:

```js
/**
 * Returns the current default value for a mob setting.
 *
 * @param {TMobType} mobType
 * @param {TMobSetting} setting
 * @returns {MobSettings<TMobType>[TMobSetting]}
 */
getDefaultMobSetting(mobType, setting)
```

```js
/**
 * Set the default value for a mob setting.
 * @param {TMobType} mobType
 * @param {TMobSetting} setting
 * @param {MobSettings<TMobType>[TMobSetting]} value
 * @returns {void}
 */
setDefaultMobSetting(mobType, setting, value)
```

```js
/**
 * Get the current value of a mob setting for a specific mob.
 * @param {MobId} mobId
 * @param {TMobSetting} setting
 * @returns {MobSettings<MobType>[TMobSetting]}
 */
getMobSetting(mobId, setting)
```

```js
/**
 * Set the current value of a mob setting for a specific mob.
 * @param {MobId} mobId
 * @param {TMobSetting} setting
 * @param {MobSettings<MobType>[TMobSetting]} value
 * @returns {void}
 */
setMobSetting(mobId, setting, value)
```

### Settings and Values for them
Here is the full list of available mob settings:

```js
/**
 * @type {"default"}
 */
variation = "default"
```

```js
/**
 * @type {string}
 */
name = ""
```

```js
/**
 * @type {number}
 */
maxHealth = 75
```

```js
/**
 * @type {number}
 */
initialHealth = 75
```

```js
/**
 * @type {string}
 */
idleSound = "pigOink"
```

```js
/**
 * @type {string}
 */
attackSound = null
```

```js
/**
 * @type {string}
 */
secondaryAttackSound = null
```

```js
/**
 * @type {string}
 */
hurtSound = "pigHurt"
```

```js
/**
 * @type { { itemName: string; probabilityOfDrop: number; dropMinAmount: number; dropMaxAmount: number; applyBurstImpulseToDrop?: boolean; }[] }
 */
onDeathItemDrops = [
    {
        itemName: "Raw Porkchop",
        probabilityOfDrop: 1,
        dropMinAmount: 1,
        dropMaxAmount: 3,
    },
]
```

```js
/**
 * @type {string}
 */
onDeathParticleTexture = "critical_hit"
```

```js
/**
 * @type {number}
 */
onDeathAura = 20
```

```js
/**
 * @type {number}
 */
baseWalkingSpeed = 3.5
```

```js
/**
 * @type {number}
 */
baseRunningSpeed = 4.55 * 0.85
```

```js
/**
 * @type {number}
 */
walkingSpeedMultiplier = 1
```

```js
/**
 * @type {number}
 */
runningSpeedMultiplier = 1
```

```js
/**
 * @type {number}
 */
jumpCount = 0
```

```js
/**
 * @type {number}
 */
baseJumpImpulseXZ = 0
```

```js
/**
 * @type {number}
 */
baseJumpImpulseY = 0
```

```js
/**
 * @type {number}
 */
jumpMultiplier = 1
```

```js
/**
 * @type {number}
 */
runAwayRadius = 0
```

```js
/**
 * @type {number}
 */
chaseRadius = 0
```

```js
/**
 * @type {number}
 */
territoryRadius = 0
```

```js
/**
 * @type {number}
 */
hostilityRadius = 0
```

```js
/**
 * @type {number}
 */
stoppingRadius = 0.5
```

```js
/**
 * @type {number}
 */
attackInterval = 0
```

```js
/**
 * @type {number}
 */
attackRadius = 0
```

```js
/**
 * @type {number}
 */
secondaryAttackRadius = 0
```

```js
/**
 * @type {number}
 */
attackDamage = 0
```

```js
/**
 * @type {number}
 */
secondaryAttackDamage = 0
```

```js
/**
 * @type {number}
 */
attackImpulse = 0
```

```js
/**
 * @type {number}
 */
secondaryAttackImpulse = 0
```

```js
/**
 * @type {string}
 */
heldItemName = null
```

```js
/**
 * @type {string}
 */
attackItemName = null
```

```js
/**
 * @type {string}
 */
secondaryAttackItemName = null
```

```js
/**
 * @type {string}
 */
attackEffectName = null
```

```js
/**
 * @type {number}
 */
attackEffectDuration = 0
```

```js
/**
 * @type {MobTameInfo}
 */
tameInfo = {
    tameItemName: [
        "Raw Porkchop",
        "Raw Beef",
        "Raw Mutton",
        "Raw Venison",
        "Cooked Porkchop",
        "Steak",
        "Cooked Mutton",
        "Cooked Venison"
    ],
    probabilityOfTame: 0.32,
    isSaddleable: false,
    foodItemNames: [
        "Raw Porkchop",
        "Raw Beef",
        "Raw Mutton",
        "Raw Venison",
        "Cooked Porkchop",
        "Steak",
        "Cooked Mutton",
        "Cooked Venison",
        "Rotten Flesh"
    ],
    foodItemsWithEffects: [
        {
            itemName: "Catnip",
            effects: [
                {
                    name: "Speed",
                    duration: 30000,
                    level: 1
                },
                {
                    name: "Damage",
                    duration: 30000,
                    level: 1
                }
            ]
        }
    ]
}
```

```js
/**
 * @type {number}
 */
onTamedHealthMultiplier = 4.0
```

```js
/**
 * @type {string}
 */
ownerDbId = null
```

```js
/**
 * @type {number}
 */
minFollowingRadius = 3
```

```js
/**
 * @type {number}
 */
maxFollowingRadius = 12
```

```js
/**
 * @type {boolean}
 */
isRideable = false
```

```js
/**
 * @type {string}
 */
metaInfo = ""
```

## Mob Types and Variations
> [!NOTE]
> From the offical documentation:

Some mob types support variations other than just `"default"`:

```js
Pig: "default"
Cow: "default", "cream"
Sheep: "default"
Horse: "default", "black", "brown", "cream"
Cave Golem: "default", "iron"
Draugr Zombie: "default", "longHairChestplate", "longHairClothed", "shortHairClothed"
Draugr Skeleton: "default"
Frost Golem: "default"
Frost Zombie: "default", "longHairChestplate", "shortHairClothed"
Frost Skeleton: "default"
Draugr Knight: "default"
Wolf: "default", "white", "brown", "grey", "spectral"
Bear: "default"
Deer: "default"
Stag: "default"
Gold Watermelon Stag: "default"
Gorilla: "default"
Wildcat: "default", "tabby", "grey", "black", "calico", "siamese", "leopard"
Magma Golem: "default"
Draugr Huntress: "default", "chainmail"
Spirit Golem: "default"
Spirit Wolf: "default"
Spirit Bear: "default"
Spirit Stag: "default"
Spirit Gorilla: "default"
```

> [!WARNING]
> This is not from the offical documentation, this was put together by NlGBOB.
> Also this has not been updated with the spirt mobs.

```json
{
  "Sheep": ["default"],
  "Stag": ["default"],
  "Wildcat": [
    "default",
    "tabby",
    "grey",
    "black",
    "calico",
    "siamese",
    "leopard"
  ],
  "Wolf": [
    "default",
    "white",
    "brown",
    "grey",
    "spectral"
  ],
  "Bear": ["default"],
  "Cave Golem": ["default", "iron"],
  "Cow": ["default", "cream"],
  "Deer": ["default"],
  "Draugr Huntress": ["default", "chainmail"],
  "Draugr Knight": ["default"],
  "Draugr Skeleton": ["default"],
  "Draugr Zombie": ["default", "longHairChestplate", "longHairClothed", "shortHairClothed"],
  "Frost Golem": ["default"],
  "Frost Skeleton": ["default"],
  "Frost Zombie": ["default", "longHairChestplate", "shortHairClothed"],
  "Gold Watermelon Stag": ["default"],
  "Gorilla": ["default"],
  "Horse": ["default", "black", "brown", "cream"],
  "Iron Golem": ["default"],
  "Magma Golem": ["default"],
  "Pig": ["default"]
}
```
