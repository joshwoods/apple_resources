

- DockKit
- DockAccessory
-  setAngularVelocity(\_:) 

Instance Method

# setAngularVelocity(\_:)

Sets the angular velocity of each axis of orientation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func setAngularVelocity(_ angularVelocity: Vector3D) async throws
```

## Parameters 

`angularVelocity`  

A Vector3D object of the angular velocity to set, in axis/angle notation, corresponsing to radians per second for pitch, yaw, and roll axes.

## Mentioned in 

Modify rotation and positioning programmatically

## Discussion

The angular velocity is expressed in radians per second for pitch, yaw, and roll. This method works only when you disable system tracking.

Throws

DockKitError.notConnected if the accessory disconnects, or other errors if communication with the accessory fails.

## See Also

### Setting position and limits

func setLimits(DockAccessory.Limits) throws

Sets limits for the axes of rotation.

func setOrientation(Vector3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setOrientation(Rotation3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

