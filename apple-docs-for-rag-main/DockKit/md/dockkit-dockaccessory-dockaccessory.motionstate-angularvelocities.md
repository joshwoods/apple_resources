

- DockKit
- DockAccessory
- DockAccessory.MotionState
-  angularVelocities 

Instance Property

# angularVelocities

The angular velocity of each axis of rotation in radians.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
let angularVelocities: Vector3D
```

## Discussion

The X, Y, and Z values are in radians per second corresponding to pitch, yaw, and roll axes.

## See Also

### Getting properties

let angularPositions: Vector3D

The angles of the axes, in radians.

let timestamp: TimeInterval

The current time, in UNIX epoch.

let error: (any Error)?

The error, if any.

