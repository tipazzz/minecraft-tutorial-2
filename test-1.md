# Spawn cows!
## Step 2

Put in ``||mobs:spawn||`` to spawn a chicken at your position.

The code under ``||player:on chat command||`` will run when you type **chicken** in the Minecraft chat.
**~0 ~0 ~0** is the relative 3D position of the player.

```blocks
player.onChat("chicken", function () {
    mobs.spawn(COW, pos(0, 0, 0))
    player.teleport(pos(0, 100, 0))
})
```

## Step 3 @fullscreen

Change the spawn position to **10 blocks** above your player.

The second number in **~0 ~10 ~0** means **10** blocks **above** of the player elevation.
The **~** symbol means that the coordinate is relative to the player.

```blocks
player.onChat("chicken", function () {
    //% highlight
    mobs.spawn(COW, pos(0, 10, 0))
})
```