

- TabletopKit
- TabletopGame
-  rootPose 

Instance Property

# rootPose

Update the root pose for the current player

visionOS 2.0+

``` source
var rootPose: Pose3D { get set }
```

## See Also

### Creating a tabletop game

init(tableSetup: TableSetup, version: Int)

Creates a tabletop game with the specified table configuration and version of rules.

func update(deltaTime: Double)

Update the game manually. Call this function if `automaticUpdate` was not set when registering the Tabletop instance.

func withCurrentSnapshot((TableSnapshot) -> Void)

