# Sound Names

## Functions to play sounds
```js
/**
 * @param {PlayerId} playerId - hears the sound
 * @param {string} soundName - Can also be a prefix. If so, a random sound with that prefix will be played
 * @param {number} volume - 0-1. If it's too quiet and volume is 1, normalise your sound in audacity
 * @param {number} rate - The speed of playback. Also affects pitch. 0.5-4. Lower playback = lower pitch
 * @param { {
 *     playerIdOrPos: PlayerId | number[]
 *     maxHearDist?: number
 *     refDistance?: number
 * } } [posSettings]
 * @returns {void}
 */
playSound(playerId, soundName, volume, rate, posSettings)
```

```js
/**
 * See documentation for api.playSound
 * @param {string} soundName
 * @param {number} volume
 * @param {number} rate
 * @param { {
 *     playerIdOrPos: PlayerId | number[]
 *     maxHearDist?: number
 *     refDistance?: number
 * } } [posSettings]
 * @param {PlayerId} [exceptPlayerId]
 * @returns {void}
 */
broadcastSound(soundName, volume, rate, posSettings, exceptPlayerId)
```

```js
/**
 * See documentation for api.playSound
 * @param {string} soundName
 * @param {number} volume
 * @param {number} rate
 * @param { {
 *     playerIdOrPos: PlayerId | number[]
 *     maxHearDist?: number
 *     refDistance?: number
 * } } [posSettings]
 * @param {PlayerId} [predictedBy]
 * @returns {void}
 */
playClientPredictedSound(soundName, volume, rate, posSettings, predictedBy)
```

## Sounds
- These are the strings you can give to functions that take a `soundName` as input
- If you want a random similar sound then you can remove the number from the sound name of your choice
- If a sound isn't working then there might be an error in your console explaining why

`beep`
`bow`
`burp`
`cashRegister`
`chestClose`
`chestOpen`
`drink`
`eat1`
`equip_leather1`
`fallsmall`
`pickUp`
`levelup`
`successfulBowHit`
`sweep6`
`trapdoorOpen`

### Firecracker
`firecracker1`
`firecracker2`
`firecracker3`
`firecracker4`

### Game Sounds
`game_start_countdown_01`
`game_start_countdow
_02` `game_start_countdown_03`
`game_start_countdown_final`

### Bucket sounds

`bucketEmpty1`
`bucketEmpty2`
`bucketEmpty3`
`bucketFill1`
`bucketFill2`
`bucketFill3`

### Bullet/Gun/Cannon sounds

`bullet_shell_bounce_general_07`
`bullet_shell_bounce_general_08`

#### Cannon

`cannonFire1`
`cannonFire2`
`cannonFire3`

#### Headshot

`headshot_04`
`headshot_06`
`headshot_08`
`headshot_11`

#### Hit

`hit1`
`hit2`
`hit3`

#### Pistol
##### Cock

`pistol_cock_01`
`pistol_cock_02`
`pistol_cock_03`
`pistol_cock_06`

##### Magazine

###### Load

`pistol_magazine_load_01`
`pistol_magazine_load_02`
`pistol_magazine_load_03`

###### Unload

`pistol_magazine_unload_01`
`pistol_magazine_unload_02`
`pistol_magazine_unload_03`

##### Shot

`pistol_shot_01`
`pistol_shot_02`
`pistol_shot_03`
`pistol_shot_04`
`pistol_shot_05`

#### Rifle
##### Cock

`rifle_cock_01`
`rifle_cock_02`

##### Magazine
###### Load

`rifle_magazine_load_01`
`rifle_magazine_load_02`
`rifle_magazine_load_03`

###### Unload

`rifle_magazine_unload_01`
`rifle_magazine_unload_02`
`rifle_magazine_unload_04`

##### Shot

`rifle_shot_01`
`rifle_shot_02`
`rifle_shot_03`
`rifle_shot_04`

#### SemiAuto

##### Cock

`semiAuto_cock_01`
`semiAuto_cock_02`
`semiAuto_cock_03`
`semiAuto_cock_04`
`semiAuto_cock_05`

##### Magazine
###### Load

`semiAuto_magazine_load_01`
`semiAuto_magazine_load_02`
`semiAuto_magazine_load_03`
`semiAuto_magazine_load_04`
`semiAuto_magazine_load_05`

###### Unload

`semiAuto_magazine_unload_01`
`semiAuto_magazine_unload_02`
`semiAuto_magazine_unload_03`
`semiAuto_magazine_unload_04`

##### Shot

`semiAuto_first_shot_01`
`semiAuto_shot_01`
`semiAuto_shot_02`
`semiAuto_shot_03`
`semiAuto_shot_04`
`semiAuto_shot_05`
`semiAuto_shot_06`
`semiAuto_shot_07`
`semiAuto_shot_08`
`semiAuto_tail_only_shot_01`

#### Shotgun
##### Cock

`shotgun_cock_01`
`shotgun_cock_02`
`shotgun_cock_03`
`shotgun_cock_04`
`shotgun_cock_05`

##### Load

`shotgun_load_bullet_01`
`shotgun_load_bullet_02`
`shotgun_load_bullet_03`
`shotgun_load_bullet_04`
`shotgun_load_bullet_05`
`shotgun_load_bullet_06`
`shotgun_load_bullet_07`
`shotgun_load_bullet_08`

##### Shot

`shotgun_shot_01`
`shotgun_shot_02`
`shotgun_shot_03`
`shotgun_shot_04`


#### Submachine
##### Cock

`submachine_cock_01`
`submachine_cock_02`
`submachine_cock_03`
`submachine_cock_04`

##### Magazine
###### Load

`submachine_magazine_load_01`
`submachine_magazine_load_02`
`submachine_magazine_load_03`
`submachine_magazine_load_04`


###### Unload

`submachine_magazine_unload_01`
`submachine_magazine_unload_02`
`submachine_magazine_unload_03`

##### Shot

`submachine_first_shot_01`
`submachine_shot_01`
`submachine_shot_02`
`submachine_shot_03`
`submachine_shot_04`
`submachine_shot_05`
`submachine_shot_06`
`submachine_shot_07`
`submachine_shot_08`
`submachine_shot_09`
`submachine_tail_only_shot_01`

### Mob Sounds
#### Golem
`golemGrunt1`
`golemGrunt2`

##### CaveGolem
`caveGolem1`
`caveGolem2`
`caveGolem3`
`caveGolem4`

#### Cow
`cowMoo1`
`cowMoo2`
`cowMoo3`
`cowHurt1`

#### Pig
##### Oink
`pigOink1`
`pigOink2`
`pigOink3`
`pigOink4`
`pigOink5`

##### Hurt
`pigHurt1`
`pigHurt2`
`pigHurt3`

#### Sheep

`sheepBaa1`
`sheepBaa2`
`sheepBaa3`
`sheepBaa4`
`sheepHurt1`

#### Dear
`deerGrunt1`
`deerHurt1`

#### Stag
`stagGrunt1`
`stagHurt1`

#### Bear
`bearRoar1`
`bearRoar2`
`bearRoar3`
`bearRoar4`
`bearRoar5`

#### Gorilla
`gorillaIdle1`
`gorillaIdle2`
`gorillaIdle3`
`gorillaIdle4`
`gorillaRoar1`

#### Dog
##### Bark
`dogBark1`
`dogBark2`
`dogBark3`

##### Growl
`dogGrowl1`
`dogGrowl2`
`dogGrowl3`

##### Hurt
`dogHurt1`
`dogHurt2`

#### Cat
##### Hiss
`catHiss1`
`catHiss2`
`catHiss3`
`catHiss4`

##### Hurt
`catHurt1`
`catHurt2`
`catHurt3`

##### Meow
`catMeow1`
`catMeow2`
`catMeow3`
`catMeow4`
`catMeow5`

#### Horse
`horseHurt1`
`horseHurt2`
`horseIdle1`
`horseIdle2`
`horseIdle3`

#### Zombie
##### Grunt

`ZombieGrunt1`
`ZombieGrunt2`
`ZombieGrunt3`

##### Hurt

`ZombieHurt1`
`ZombieHurt2`
`ZombieHurt3`
`ZombieHurt4`

#### Knight
`knightGrunt1`
`knightGrunt2`
`knightGrunt3`

#### Skeletion
`skeletonRattle1`
`skeletonRattle2`
`skeletonRattle3`
`skeletonRattle4`

### Door Sounds

`doorClose`
`doorClose2`
`doorOpen-bloxd1`
`doorOpen-bloxd2`

### XP Sounds

`exp_collect`
`exp_levelup`

### Glass Sounds

`glass1`
`glass2`
`glass3`

### Cloth

`cloth1`
`cloth2`
`cloth3`
`cloth4`

### Grass Sounds

`grass1`
`grass2`
`grass3`
`grass4`

### Gravel Sounds

`gravel1`
`gravel2`
`gravel3`
`gravel4`

### Hoe Sounds

`hoeTill1`
`hoeTill2`
`hoeTill3`
`hoeTill4`

### Sand

`sand1`
`sand2`
`sand3`
`sand4`

### Snow

`snow1`
`snow2`
`snow3`
`snow4`
`splash1`

### Step
#### Cloth

`step_cloth1`
`step_cloth2`
`step_cloth3`
`step_cloth4`

#### Grass

`step_grass1`
`step_grass2`
`step_grass3`
`step_grass4`
`step_grass5`

#### Gravel

`step_gravel1`
`step_gravel2`
`step_gravel3`
`step_gravel4`

#### Sand

`step_sand2`
`step_sand3`
`step_sand4`
`step_sand5`

#### Snow

`step_snow1`
`step_snow2`
`step_snow3`
`step_snow4`

#### Stone

`step_stone1`
`step_stone2`
`step_stone3`
`step_stone4`
`step_stone5`
`step_stone6`

#### Wood

`step_wood1`
`step_wood2`
`step_wood3`
`step_wood4`
`step_wood5`
`step_wood6`

### Stone

`stone1`
`stone2`
`stone3`
`stone4`

### Wood

`wood1`
`wood2`
`wood3`
`wood4`

### Bass

`bass`
`bassattack`

### Misc

`bd`
`harp_pling`
`hat`
`snare`
