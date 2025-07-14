

- DockKit
- DockAccessory
-  setLimits(\_:) 

Instance Method

# setLimits(\_:)

Sets limits for the axes of rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func setLimits(_ limits: DockAccessory.Limits) throws
```

## Parameters 

`limits`  

The upper and lower limit of orientation, in radians, for each of the supported axes.

## Discussion

Limits only apply to the current tracking session. Afterwards, the orientation specifications default to the manufacturer limits. This method impacts primarily subsequent calls to setOrientation(_:duration:relative:) and setOrientation(_:duration:relative:). Limits only apply to the current tracking session. When the session ends, the orientation specifications default to the manufacturer limits.

This method only works when you disable system tracking.

Throws

An error if all parameters are `nil`, or if the dock accessory doesn’t support the given axis.

## See Also

### Setting position and limits

func setOrientation(Vector3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setOrientation(Rotation3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setAngularVelocity(Vector3D) async throws

Sets the angular velocity of each axis of orientation.

