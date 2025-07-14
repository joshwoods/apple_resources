

- TabletopKit
- TabletopGame
-  update(deltaTime:) 

Instance Method

# update(deltaTime:)

Update the game manually. Call this function if `automaticUpdate` was not set when registering the Tabletop instance.

visionOS 2.0+

``` source
func update(deltaTime: Double)
```

## See Also

### Creating a tabletop game

init(tableSetup: TableSetup, version: Int)

Creates a tabletop game with the specified table configuration and version of rules.

var rootPose: Pose3D

Update the root pose for the current player

func withCurrentSnapshot((TableSnapshot) -> Void)

