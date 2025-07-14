

- DockKit
- DockAccessory
-  setOrientation(\_:duration:relative:) Deprecated

Instance Method

# setOrientation(\_:duration:relative:)

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

iOS 17.0–18.0DeprecatediPadOS 17.0–18.0DeprecatedMac Catalyst 17.0–18.0DeprecatedmacOS 14.0–15.0Deprecated

``` source
final func setOrientation(
    _ rotation: Rotation3D,
    duration: Duration = .seconds(0),
    relative: Bool = false
) throws -> Progress
```

Deprecated

please use async version of setOrientation

## Parameters 

`rotation`  

The spatial framework’s Rotation3D with X, Y, and Z corresponding to radians of pitch, yaw, and roll axes.

`duration`  

The duration, in seconds, to reach the target orientation.

`relative`  

Calculate the relative-to-current positions, if set to `true`; otherwise, move to an absolute position.

## Return Value

A progress object that reports the progress towards the target orientation.

## Mentioned in 

Modify rotation and positioning programmatically

## Discussion

This method works only when you disable system tracking.

Throws

DockKitError.frameRateTooHigh if calling the method too frequently, or DockKitError.notSupported in macOS.

## See Also

### Setting position and limits

func setLimits(DockAccessory.Limits) throws

Sets limits for the axes of rotation.

func setOrientation(Vector3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setAngularVelocity(Vector3D) async throws

Sets the angular velocity of each axis of orientation.

