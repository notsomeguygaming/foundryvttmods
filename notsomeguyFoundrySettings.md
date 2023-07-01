## `generating config from blank base`
- update user permissions
- manage modules
- configure module settings
- token mold
- export

## `setup in new world with preset config`
- activate mod forien-copy-environment
- `right click` game version on top right
- click `export` to save current world settings
- click `import` and select the premade json from forien-copy-environment 
- reload the game a couple times for user settings to fully apply
### `configure game settings (default/recommended)`
- `W` world setting(gm)
- `WO` world optional setting
- `U` user setting
- `UO` user optional
- `UG` user graphics setting for performance
- `default / recommended` (UG low end may want off)
    - `+` check
    - `-` uncheck
- core
    - W configure user permissions `(img)`
    - UO left click to release objects  -/+
    - UG token vision animation +/+
    - UG light source animation +/+
    - W animate roll tables    +/-
- dnd5e
    - WO allow polymorphing -/+
- action pack
    - UO tray display mode   `automatic / toggle`
        - only really affects GM as players will always be `toggle` regardless of setting
- active-auras
    - WO auras in combat -/-
- always hp
    - UO clear after applying +/+
- automated automations
    - W 
        - delete `call lightning(templates)`
        - preset `misty step` movement options `token alpha` to 1, also affects `starlight step`
        - possibly also set (preset) `dimension door,far step, teleport, thunderstep`
        - delete `fog cloud(templates)` unless using `dnd5e-animations`
        - delete `witch bolt(preset)`
        - delete `aura of (auras)`
        - set `spirit guardians(auras)` volume to 0.1
        - if animation stuck `Use the Tile Foreground Layer to remove the Animation`
        - if stuck can also check Sequencer.EffectManager.show()
    - UG automated automations  `on/off`
- combat carousel
    - U collapse navigation bar (good for gm) -/+
    - U open the combat carousel on combat creation -/+
    - U carousel size   `medium/small`
- damage log
    - W allow players to view the damage log    -/+
    - W minimum actor permission    `owner/limited`
- dfreds convenient effects 
    - W (`import` custom effects from `sidebar icon` if have file, mostly because some light is too bright)
    - W app controls permission     `game master / trusted player`
- dfreds effects panel
    - UO show disabled effects   +/+
    - UO show passive effects   -/+
    - UO passive effects right click behavior (maybe `delete` if you have an effect with a measured template that you need to delete instead of disable at the end of the turn)  `disable / disable`
- dice so nice
    - UO 3d dice settings   customize dice
- dnd5e drag ruler integration
    - UO hide switch speed button  (OFF if you have an alternate speed like flying) -/+ 
    - U hide toggle terrain button  (don't really need to toggle it)   -/+
- drag ruler
    - W show GM ruler to players   +/-
    - W allow pathfinding for players   -/+
    - U pathfinding by default (for players, dm off otherwise can't move tokens over walls) -/+
- drag upload
    - W change path to `dragupload/uploaded/myname/myworld`
- dungeon draw
    - W allow trusted players   +/-
- follow me
    - W snap to grid	-/+
    - W test for collisions		-/+
    - W stop following in combat	-/+
- forien's quest log
    - W allow player reward dragging (gm still needs to make visible and unlock) -/+
    - W players can create quests   -/+
    - W players can accept quests   -/+
    - W allow trusted player quest editing  -/+
    - W default quest permission level  `observer/owner`
    - W show reward drop notifications  -/+
- hey wait
    - W restrict GM from triggering tiles   -/+
- initiative-double-click
    - W minimum permission level `gamemaster / trusted player`
- midiqol `(img)`
    - W choose critical damage   `dnd settings only / max critical dice(rolldice)`
    - WO add damage buttons to char message     `none / only add buttons for GM`
    - W colored border messages     `none / border only`
- monks combat details
    - W prevent spell changes   `show chat message/ignore`
    - W show start token    +/-
    - W hide enemies    -/+
    - W hide until turn     -/+
    - UO volume (your turn notification)    `60/60`
- monks hotbar expansion
    - U number of rows  `5/3`
    - U reverse     -/+
    - U hide the first row    -/+
    - U start collapsed    +/-
    - U collapse on select +/-
    - U hide page arrows    -/-
- monks player settings
    - U sync settings  (only activate on player first run then deactivate) +/-
- monks tokenbar
    - W allow player to use    -/+
    - WO double click action     `open character sheet / request saving throw / open character sheet`
    - W notify on movement change   +/-
    - W change movement to combat   +/-
    - W whisper player on level up  +/-
    - W show xp dialog  +/-
- monsterblock
    - W hide image    -/+
- party overview
    - WO grant players access to the overview    +/-
- quick insert
    - W index settings `(img)`
- quickscale
    - W range   0.8-1.2 / 2.8-3
    - W maximum rotation amount     15 / 0
- rarity colors
    - W spell color     +/-
    - W feat color     +/-
        - U Spell color         `#4a8396 / blank`
        - U Spell external color        `#0000ff / blank`
        - U Feat color      `#48d1cc / blank`
- rest recovery
    - W configure rest -> long rest -> 
        - W enable exhaustion automation    -/+
        - W exhaustion module integration   `none / dfreds convenient effects`
        - W hit dice recovery fraction      `half / full`
- sequencer
    - U show sequencer tools    +/-
    - U show sequencer tools in token controls   +/-
    - UG enable effects     +/-
    - W sequencer: use sidebar tools    `players and above / assistant gms and above`
    - if there are any issues with effects use macro Sequencer.EffectManager.show()
- shared vision
  - W configuration -> `limited` -> `token`  (if you want to let players see the token but not the sheets)   -/+
  - WO configuration -> `limited` -> `vision` (if you want to let players see vision but not the sheets)    -/+
- simbuls creature aide
    - W config
        - W ability recharge-> automatically roll ability recharge      `off / start of turn`
        - W lair action -> lair prompt  (be sure to make a lair action on the char sheet)`(img)` -/+
        - W legendary action->start of turn legendary action  -/+
- simbuls template scaling
    - W auto adjust templates to 5e grids (fixes diagonals)      `no template scaling / lines and cones`
- simbuls wild surges
    - W wild magic auto detect  `disabled / enabled`
    - W wild magic surge table name DO NOT USE 10000 wild surges unless you have core->animate roll tables unchecked, it's not even a good list 
        - (drag into hotbar and edit for name ex: Compendium.foundry_community_tables.community-tables-independent.5uRCMR11qY2Dwrw9 or use regular name in tables list [Wild Magic Surges])
        - alternatively create a table called `wild` and drag in [`wild magic surges, moderate, nuisance, extreme`]   
        - Wild-Magic-Surge-Table / `wild`
    - W recharge tides of chaos on surge    -/+
    - U on character sheet of wild magic player under configure special traits, set wild magic type
        - `standard` is on 1
        - `more` is equal or lower than spell level cast
        - `Volatile` similar to `more`, but adds 1d4 to the spell level if Tides of Chaos has been expended
        - `accumulating` starts at 1 and increases by 1 every cast
    - W table roll mode     `default / public roll`
- simple calendar
    - U open on load    +/-
        - should basically auto close after first run if smalltime is on anyway
- smalltime
    - W small step amount   `10-10`
    - W large step amount   `60-60`
    - W affect darkness by default  -/+
    - WO moon phase affects darkness    -/-
- tactical grid
    - UG disable tactical grid      -/+
    - U display distances on ruler drag  (if you don't want to use the keybind)   -/+
    - UO in keybinds add button for `display distances`
- times up
    - WO disable passive effects on expiry  -/-
- token action hud
    - U direction   `up / down`
- token info icons
    - W gm only     +/-
- token magic fx
    - we don't need animations for this is using autoanimations but need need it on for auto wounds
    - W enable automatic template effects +/-
    - UG disable fx animations  -/+
    - W disable video support in templates -/+
- tokenizer
    - W add a frame to the token when opened    +/-
- token mold
    - W actors -> settings -> name -> choose adjectives from the following rollable table   `english set of 700` / `english over 4700 random`
- windows controls
    - U organized minimize    `top / bottom taskbar`

## `user only (default/recommended)`
- <span style="background:ivory">![_____](tags/ivory.png)</span>action pack
    - U tray display mode   `automatic / toggle`
        - only really affects GM as players will always be `toggle` regardless of setting
- core
    - UO left click to release objects  -/+
- combat carousel
    - U open the combat carousel on combat creation -/+
    - U collapse navigation bar (good for gm) -/+
    - U carousel size   `medium/small`
- dfreds effects panel
    - UO show disabled effects   +/+
    - UO show passive effects   -/+
    - UO passive effects right click behavior (maybe if you have an effect with a measured template that you need to delete instead of disable at the end of the turn)  `disable / disable`
- <span style="background:ivory">![_____](tags/ivory.png)</span>dice so nice
    - UO 3d dice settings   customize dice
- dnd5e drag ruler integration
    - UO hide switch speed button  (OFF if you have an alternate speed like flying) -/+ 
    - U hide toggle terrain button  (don't really need to toggle it)   -/+
- <span style="background:ivory">![_____](tags/ivory.png)</span>drag ruler
    - U pathfinding by default (for players otherwise need to use hotkey, dm off otherwise can't move tokens over walls and dm can't use hotkey) -/+
- <span style="background:ivory">![_____](tags/ivory.png)</span>drag upload
    - W change path to `dragupload/uploaded/myname/myworld`
- monks combat details
    - UO volume (your turn notification)    `60/60`
- <span style="background:ivory">![_____](tags/ivory.png)</span>monks hotbar expansion
    - U number of rows  `5/3`
    - U reverse     -/+
    - U hide the first row    -/+
    - U start collapsed    +/-
    - U collapse on select +/-
    - U hide page arrows    -/-
- monks player settings
    - U sync settings  (only activate on player first run then deactivate) +/-
- simbuls wild surges
    - U on character sheet of wild magic player under configure special traits, set wild magic type
        - `standard` is on 1
        - `more` is equal or lower than spell level cast
        - `Volatile` similar to `more`, but adds 1d4 to the spell level if Tides of Chaos has been expended
        - `accumulating` starts at 1 and increases by 1 every cast
- simple calendar
    - U open on load    +/-
        - should basically auto close after first run if smalltime is on anyway
- <span style="background:ivory">![_____](tags/ivory.png)</span>tactical grid
    - U display distances on ruler drag  (if you don't want to use the keybind)   -/+
    - UO in keybinds add button for `display distances`
- <span style="background:ivory">![_____](tags/ivory.png)</span>token action hud
    - U direction   `up / down`
- <span style="background:ivory">![_____](tags/ivory.png)</span>windows controls
    - U organized minimize    `top / bottom taskbar`
## `user low graphics only (default/recommended)`
- core
    - UG token vision animation +/-
    - UG light source animation +/-
- automated automations
    - UG automated automations  `on/off`
- dice so nice
    - UG 3d dice settings
        - UG preferences -> enable immersive darkness mode     +/-
        - UG performance -> image quality      `high / medium`
- sequencer
    - UG enable effects     +/-
- tactical grid
    - UG disable tactical grid      -/+
- token magic fx
    - UG disable fx animations  -/+
```
Enable Hardware Acceleration
If you've been experiencing performance issues, grey backgrounds, or scenes are not rendering, follow these steps in the affected player's browser:
Browser Hardware Acceleration Settings

Chrome, Chromium, Edge -
1. Open chrome://settings, enable Use Hardware Acceleration When Available
2. Open chrome://flags, enable Override Software Rendering List
3. Fully close and re-launch Chrome.

Firefox -
1. Open about:config , set layers.acceleration.force-enabled to true
2. Fully close and re-launch Firefox.
```
## `Permissions`
### `actor` - limited for only showing the token icon (secret game), observer for checking items and abilities
| permission | select | sheet view | edit | share | in list |
|:----------:|:------:|:----------:|:----:|:-----:|:-------:|
| none       |    X   |     X      |   X  |   X   |    X    |
| `limited`  |    X   |   `icon`   |   X  |   X   |  `O`    |
| `observer` |    X   |   `stats`  |   X  |   X   |  `O`    |
| owner      |  `O`   |   `stats`  | `O`  | `O`   |  `O`    |
### `item` - none so it's not in the list
| permission | select | open view | view stats | edit | share | in list | secretText |
|:----------:|:------:|:---------:|:----------:|:----:|:-----:|:-------:|:----------:|
| `none`     |    X   |     X     |     X      |   X  |   X   |    X    |      X     |
| limited    |    X   |     `O`   |     X      |   X  |   X   |    `O`  |      X     |
| observer   |    X   |     `O`   |     `O`    |   X  |   X   |    `O`  |      X     |
| owner      |    `O` |     `O`   |     `O`    |   `O`|   `O` |    `O`  |      `O`   |
- secret text does not show up in chat unless `revealed`
- items in inventory are set to `owner`, will not see in list unless explicitly changed
### `journal` - limited so it's not in the list
- if `show players` is clicked on the journal, document will be shown with journal level permission
    - if the journal is `none` and all pages are `none`, every page will be shown
- if `show players` is clicked for the `page`, page will be shown regardless of permission

|J permission | select | read pg lim | read pg obs | edit | share | in list | secretText |
|:-----------:|:------:|:-----------:|:-----------:|:----:|:-----:|:-------:|:----------:|
| none        |    X   |       X     |       `O`   |   X  |   X   |    X    |      X     |
| `limited`   |    X   |       X     |       `O`   |   X  |   X   |    X    |      X     |
| observer    |    X   |       `O`   |       `O`   |   X  |   X   |    `O`  |      X     |
| owner       |    `O` |       `O`   |       `O`   |   `O`|   `O` |    `O`  |      `O`   |

# `importing steps`
- use `forien-copy-environment` or `midiqol` import to restore config
    - activate `forien-copy-environment` mod
    - `right click` on game version on right side above mod configs and click import
    - skip `compendium-folders`
- dnd5e-animations may ask if you want to update all animations, click update
### `configure after import game settings`
- drag upload
    - W change path to `dragupload/uploaded/myname/myworld`
- dfreds convenient effects 
    - W `import` custom effects from `sidebar icon` if haven't already. contains `[dodge, faerie fire, light, torch]`
- item pile
    - drop any item onto canvas to create `default item pile` 
        - `set Default Item Pile` interaction distance to be more than 1
        - `item pile` is a list of items and their amount
        - `container` is item pile but lets you change image for the pile if it's open or closed or locked
        - `merchant` lets a player buy and sell from the token
        - `vault` is a mini grid for items to sit in
- sharedvision
    - change `limited` vision type to `fog` `token` or `vision`
- token mold
    - set categories to randomize (name only)
- z-scatter
    - size snap button `on` in left panel
- configure any keybinds
- configure individual user settings
- `mountup` set token you want to be the mount, `on` in prototype token
### `Other Notes`
- vision modes in token configuration ->vision
    - Basic Vision
        - no effect on filter regardless of light
        - still limited by range
    - Darkvision
        - areas that are illuminated by light are in full color
        - areas that are not illuminated by light are filtered in greyscale
    - Monochromatic
        - similar to Darkvision by all areas are filtered in greyscale
    - Tremor Sense
        - creates a radar-like filter that pulses around the token and walls
        - does not allow a token to sens other tokens, must be done in detection mods tab
    - Light Amplification
        - bright filter over token's vision, looks visually like nightvision
    - To make a token `blind`, you need the `perfect vision` mod and change token vision range in darkness and light to 0
- scene configure->lighting->`global illumination` brightens the whole map, so does turning off token vision
    - In order to simulate daytime, you use the function Global Illumination. What that does is allow all tokens with Vision to see as far as they possibly can, but their vision can still be limited by walls.
    - turning off token vision allow all tokens to see as far as they possibly can not limited by walls
- PCs cannot see the vision of tokens with `limited` permission, nor the stats. 
- PCs can see the vision of tokens with `observer` permission, as well as the stats. 
- if you want tokens to have vision on the scene without global illumination, either `add lights to the map` or set the prototype token `vision`->`vision radius(in darkness)` -> `60`
- `right click` status icons to make them fill the entire token instead of just the corner
- create a token for lair actions and set to init 20 or drag/create a feature on the sheet with type `lair action`
- lair actions don't seem to have been imported
- configure settings->core->`pan token to speaker`
- `double right click` targets a hostile token
- drag a token onto another character sheet to perform a `polymorph`, use `restore transformation` at top of character sheet to revert
- on `actors` button, create a token type `group` and add tokens to see `total hp` of tokens, set `permissions` so all can see. inventory is `copy` based
### `quick mod hotkey controls`
- aedifs-tactical-grid
    - use `drag` or `hotkey` to see distance of other tokens
- arbron-summoner
    - on the `summoner's sheet`-> features -> new feature with action type `summoning`, drag summon token onto blank square under `summons`
    - on `token sheet you want to summon`, click `summon configuration`, turn on `match proficiency` and `match to hit`
- easy-target
    - hold `alt` and `leftclick / drag` tokens to `target` them
    - hold `alt` and `leftclick` empty space to `deselect` all
- followme
    - To start following select your token, hold the mouse pointer over whom you wish to follow and press `F`.
- monks-wall-enhancement
    - hold `ctrl` to draw more walls
    - hold `alt` to join wall ends
    - `double click` to create a new wall point
    - `ctrl rightclick` on a secret door turns it into a regular door `if not using smart doors`
- monks-active-details 
    - hold `M` then `left click` to move selected characters
- monks-tokenbar
    - `left click` on token once to pan to it
    - to add token to bar, `right click` token -> config -> `show on tokenbar`
- multi-token-edit
    - Common data shared between all placeables will be highlighted as `green`, 
    - differing data as `orange`, 
- permission_viewer
    - none - `3 dots`
    - limited - `diamond`
    - observer - `square`
    - owner - `circle`
- quick-insert 
    - `ctrl + shift` popup
    - `@` narrow search
- quickscale
    - `]` enlarge token
    - `\` reset token size to prototype
- simbuls-cover-calculator 
    - select token, hover target, `R`
- smart-doors
    - `alt+left click` a door toggles regular/secret door
- sweetnothings
    - whispers `alt + w`
    - reply `alt + r`
