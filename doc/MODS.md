# Available modifications

## Challenge

### Time limit

Select the `GameLogic` node. From the Inspector, under `Challenges`, you
can set a time limit. The player must achieve the win condition(s) before
the specified time elapses, otherwise they lose.

### Number of lives

Select the `GameLogic` node. From the Inspector, under `Challenges`, you
can customise the number of lives. The player will lose a life every time
they touch an enemy or fall off the world. When no lives are remaining,
the player has lost the game.

## Core Mechanics

### Gravity

Select the `GameLogic` node. From the Inspector, you can adjust the
Gravity of the world. Decreasing gravity will allow the player to jump
higher.

## Rules

### Win condition

Select the `GameLogic` node. From the Inspector, under `Win Condition`,
you can adjust the conditions needed to win the game. You can either require
the player to collect a certain number of coins, or reach a flag, or both.

## Space

### Designing the level

Select the `TileMap` node. The TileMap bottom panel will appear. From
there, click on the Paint tool ✎ if it is not already selected. Click on
a tile from the bottom section (or click-and-drag to select several). Now
you paint those tiles by simply clicking on the main 2D canvas.

To erase elements of the level, the Eraser tool can be selected in the
TileMap panel at the bottom, then click on the parts of the level in the
canvas view to remove them.

In the TileMap panel, click Patterns to view some predefined tile patterns
for easy creation of platforms within the game. To create more patterns,
click the Selection tool (to the left of Paint) in the TileMap panel, then
select a group of tiles from the main 2D canvas view, and drag them into
the Patterns area.

the canvas above. Other tools like the Eraser can be handy for
designing your own level.

### Tinting the background

Select the `Background` node. In the inspector, click the `Tint` colour bar
and you can adjust the tint applied to the background. This gives your game
a whole new feel.

### Alternative world visuals

Select the `TileMap` node. In the Inspector, look carefully to the right of
where it says `Tile Set`, you will see a down arrow ⌄. Click that small
arrow, and click `Quick Load`. Now you can select between 4 different
tilesets. Changing tilesets will 're-skin' your existing level with a
different visual style which will give it an entirely different feel.

## Components

### Coins

Click an existing coin in the level and observe that it selects one of the
Coin nodes in the Scene Dock. Now press `Ctrl+D`. It may appear that nothing
has happened, but you have actually duplicated the coin and it is sitting
directly on top of the original. Click and drag the coin and you will see
that you have added a coin to the game which you can position to your liking.

### Enemies

Click on an Enemy in the level. In the Inspector, you can adjust:
- The enemy's `Speed`
- Whether they `Fall Off Edges`
- Whether the `Player Loses Life` when touching it
- Whether they are `Squashable` by the player jumping on top of them
- The left vs right `Start Direction`.

In the 2D canvas you can also reposition these enemies and adjust their
size with the Scale Mode tool.

### Dynamic platforms

The sample level comes with several dynamic platforms under `Platforms`. Click
on one of these nodes. In the Inspector, you can adjust their behaviour:

- `Width` can be adjusted to make them larger.
- A `One Way` platform can be reached by jumping through it from below and
  then landing on it. A platform that is not `One Way` will act as a solid
  object if you jump at it from below. Setting or unsetting this changes the
  visual appearance of the platform accordingly.
- The `Fall Time` configures how long the platform remains in the world
  before it falls away. A `Fall Time` of -1 means that the platform is static.

These platforms can be made into moving platforms by using Godot's Animation
functionality.

### Player and flag appearance

Click on the `Player` node. In the inspector, observe where it says `Sprite
Frames`. To the very right, there is a small down arrow ⌄. Click this, and
click `Quick Load`.

You will now see a list of 6 resources. 2 of them are for the flag, and 4
apply to the player. Click on a different player resource and observe that
your player now looks rather different. Each player resource has a different
appearance and animation.

The same customisation can be done on the `Flag` node, by selecting that one,
and using the `Sprite Frames` `Quick Load` to select the alternative flag
design.