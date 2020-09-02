# TITLE
## Step 2

Put in ``||mobs:spawn||`` to spawn a chicken at your position.

The code under ``||player:on chat command||`` will run when you type **chicken** in the Minecraft chat.
**~0 ~0 ~0** is the relative 3D position of the player.

```blocks
player.onChat("chicken", function () {
    mobs.spawn(CHICKEN, pos(0, 0, 0))
})
```

## Step 3 @fullscreen

The ``||loops:for||`` loop tells the computer to repeat the code under it.

```blocks
player.onChat("square", function () {
    for (let i = 0; i <= 3; i++) {
        agent.move(FORWARD, 3)
        agent.turn(LEFT_TURN)
    }
})
```