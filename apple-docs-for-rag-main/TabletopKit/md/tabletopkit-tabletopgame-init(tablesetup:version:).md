

- TabletopKit
- TabletopGame
-  init(tableSetup:version:) 

Initializer

# init(tableSetup:version:)

Creates a tabletop game with the specified table configuration and version of rules.

visionOS 2.0+

``` source
@MainActor
init(
    tableSetup: TableSetup,
    version: Int = 0
)
```

## Parameters 

`tableSetup`  

The initial arrangement of seats, equipment, and counters during gameplay.

`version`  

The version of rules for this game.

## Discussion

Players can only join multiplayer games when their rules version matches other players.

## See Also

### Creating a tabletop game

var rootPose: Pose3D

Update the root pose for the current player

func update(deltaTime: Double)

Update the game manually. Call this function if `automaticUpdate` was not set when registering the Tabletop instance.

func withCurrentSnapshot((TableSnapshot) -> Void)

