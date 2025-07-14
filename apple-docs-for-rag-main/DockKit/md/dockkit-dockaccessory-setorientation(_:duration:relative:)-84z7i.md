

- DockKit
- DockAccessory
-  setOrientation(\_:duration:relative:) 

Instance Method

# setOrientation(\_:duration:relative:)

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
final func setOrientation(
    _ rotation: Vector3D,
    duration: Duration = .seconds(0),
    relative: Bool = false
) async throws -> Progress
```

## Parameters 

`rotation`  

The spatial framework’s Vector3D with X, Y, and Z corresponding to radians of pitch, yaw, and roll axes.

`duration`  

The duration, in seconds, to reach the target orientation.

`relative`  

Calculate the relative-to-current positions, if set to `true`; otherwise, move to an absolute position.

## Return Value

An object that reports progress during the animation sequence.

## Discussion

This method works only when you disable system tracking.

Throws

DockKitError.frameRateTooHigh if calling the method too frequently, or DockKitError.notSupported in macOS.

