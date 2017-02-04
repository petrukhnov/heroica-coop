# heroica-coop

Alternative rules to convert Lego Heroica game from competitive to coop. Best for 2-4 players.  Possible to play with more players, but it will increase wait time.


# Why

Give possibility to play as team and have kind of progression between games. 

# Main differences

- common goal
- random gameboard
- random location of enemies and loot
- permadeath
- difficulty options 
- not possible to buy weapons during game
- require more pieces to play (e.g. more sets, or just extra bricks)
- GM may present

## Playing with GM

If GM is present, he could enhance story, controll enemies, and help with maze building.

# Game setup

1. Selecting quest for game
1. Character selection and shopping
1. Placing starting area
1. Game (turns)
1. Rewards, shopping and saving characters

## Game difficulty

Here and later all dice values will be presented as 1-4 values (4 is for shield). 

```
Peaceful 133344 (very easy, and don't provide any rewars at the end)
Easy 123344
Normal 122334 (default heroica dice)
Hard 112234
Impossible 122233 (no shield here)
```

Difficulty also provide better results at the end. 

### Rewards

When quest is completed, and everyone left maze, each survived player throw dice to get reward:

```
Reward:
  E  N  H   I
1 -  1g 2g  1g+W
2 -  -  1g  2g
3 1g 1g W   W+W
4 1g 2g M   - 

g - gold
W - wepon of his choice
M - access to new maps (e.g. story, quests, etc)
```

## Quest selection

Quests:

- defeat all enemies in maze
- visit all big islands
- rescue someone from jail (not implemented yet)
- defeat boss or several
- etc

## Character selection

Players could select characters from previousely saved ones, or use new character. New characters always start without any items, and normal difficulty is recommended. When players know quest and difficulty, they may adjust charcter selection to fit better.

### Characters

Type (Color) - shield skill, favourite weapon (special weapon skill)

 - Barbarian (Yellow) - kill all + move 1 space, battle axe (repeat if more enemies)
 - Wizard (Red) - kill ranged 3 +corners, wand (range 5)
 - Druid (Brown) - heal all by 1 in 1 range, staff (by 2 range 2, or same room)
 - Ranger (Blue) - kill 5 straignt, bow (shoot twice)
 - Rogue (Green) - kill and search (sh=2g), dagger (single sword also work)
 - Prince (Blue) - kill and move 2 spaces, sword (single sword also work)
 - Sage (White) - pick item 3 spaces away, staff (4 spaces away)
 - Priest (White) - heal 2 (1 range), staff (heal all, range 3)
 - Gladiator (Red) - move 1 and kill over 1 cell, spear (move 0-1 after kill)
 - King (Yellow) - give action to any other character, sword (act, and then give action)

Usually it is good idea to have different colors for minifigs, but adding round tile on top may hellp to distinguish.

E.g. there Barbarian with battle axe and bow, having 3 enemies in front of him. If shield comes, he may use battleaxe to rush through all 3 enemies, defeting all of them, without extra dice trowing.

```
todo: dark side
```

### Weapons

Weapon is weaker than character skill

- Bow - kill 4 ranged
- Battle axe - kill all
- Staff - heal 1 range 1
- Wand - kill range 3
- Sword - move 1 and kill
- Dagger - kill and search (sh=1g)
- Spear - kill moster over 1 cell

### Potions

- red(1) - restore 2 health
- yellow(2) - defeat monster
- green(3) - prevent health loss
- blue(4) - throw potion up to 3 cells on empty space, monsters run 3 spaces away (if possible)

```
todo:
purple
orange
white
black
empty
```

## Placing starting area



### Initial location
starting room, 2 bridges and 2 small islands, 1 button, 1 enemy

## Game entities

Labyrynth size and how much items you should have:

- S (15 min) - 1 big island, 5 small, 8 bridges (1 heroica set)
- M (30 min) - 2 big islands, 8 small, 16 bridges  (1.5 heroica set)
- B (75 minutes) - 5 big islands, 15 small, 30 bridges (3 heroica sets)
- Sky is the limit (8 hours) - enough items
- Sky is not the limit

### Map elements

 - bridge (long/short/T-shape, 2-4 tiles) 
 - small island (6x6 plate, 3-4 tiles)
 - big island (8x8 plate, 6-9 tiles)
 
 Elements maybe prepared before game.
 
### Enemies

- spider, bat (animals): strength 1
- monster, zombie (tinyfigs): strength 2
- mage, vampire (tinyfigs with additions): strength 3
- vampire dragon-bat, other combined creatures: strength varies

## Game

Similar rules as base game. Turns, fights, etc. If player lost all health, he dies, and can't participate in this game anymore. If player leave labyrinth in the middle of game, he can't participate in game (but may be eligeble for reward).

If players haven't completed quest, they will not get reward at the end, but may keep items that are on character.

### GM

If playing with GM: on his turn, he could move 1 monster:

Throw dice:

- 1 - closest to heroes, move to sword direction
- 2 - closest to heroes, move 2 tiles towards hero
- 3 - further away from heroes, move to sword direction
- 4 - no move

If enemy end his turn close to hero, GM throw dice:

 - 1 - hero wounded and step back, monster defeated
 - 2 - hero wounded and step back
 - 3 - monster defeated
 - 4 - monster defeated

### Search walls

When player defeat last visible enemy in Labyrinth, he may add bridge and island to same or adjustent room, where he is.

Also player may spend his turn to search for hidden passage. Player should be on island, and no monsters should be on that island.

Adding new islands to maze: 

- 1 - nothing (mark 1 island size as closed)
- 2 - nothing (mark 1 island size as closed)
- 3 - small island + bridge
- 4 - big island + bridge

If nothing found during search, block one of the sides in room with 2x1 brick.  

If island - add bridge (roll dice) and prepared island.

If no suitable island, replace with available. If no islands, could build bridges (if still available).

After island placed, roll dice: 
```
Small
1 - 2 monsters (str: 1,2), 1 item
2 - 2 monsters (str: 2,1), 0 items
3 - 1 monster (str: 2), 1 item
4 - 1 monster (str: 1), 2 items
Big: 
1 - 3 monsters (str: 2,3,1), 1 items
2 - 4 monsters (str: 2,2,2,3), 0 items
3 - 2 monster (str: 2,3), 2 items
4 - 2 monster (str: 1,3), 3 items
Additionally big island have quaest item, or chalice (worth 3 gold)
```

All items always on islands (except buttons, and gates). 1st monster always on bridge

Roll for each item:
1 - gate or button (gates can't be more than buttons, buttons can't be more than gates x 3).
2 - chest
3 - 1g
4 - potion (roll for potion type)

If GM present, he could place items based on his will.


# Rewards, shopping and saving characters

If quest completed, all survived characters may roll for reward. 

Character progression is saved per character per player. E.g. if one player have Wizard with 3 gold and bow at the end, it is recorded, and next game when he starts with Wizard, he get same items. Other players may have own saved Wizards, or other characters. When player defeated, his recorded character is cleared.


