# Spawn mobs

## Introduction @unplugged

Spawn a bunch of mobs!

## Step 1

Drag in an ``||player:on chat command||`` and rename it to **mobs**.

```blocks
player.onChat("mobs", function () {
})
```

## Step 2

Put in ``||mobs:spawn||`` to spawn some mobs at your position.

```blocks
player.onChat("mobs", function () {
    mobs.spawn(COW, pos(0, 0, 0))
})
```

## Step 3

Go to Minecraft and enter `mobs` in the chat to spawn mobs!


```ghost
player.onChat("square", function () {
    agent.teleportToPlayer()
    for (let i = 0; i <= 3; i++) {
        agent.move(FORWARD, 3)
        if (agent.detect(AgentDetection.Block, FORWARD)) {
            agent.turn(RIGHT_TURN)
            agent.move(FORWARD, 1)
        } else {
            agent.turn(LEFT_TURN)
        }
    }
})
```