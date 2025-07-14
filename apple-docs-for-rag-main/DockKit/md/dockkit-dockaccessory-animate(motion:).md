

- DockKit
- DockAccessory
-  animate(motion:) 

Instance Method

# animate(motion:)

Starts an animation sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func animate(motion: DockAccessory.Animation) async throws -> Progress
```

## Parameters 

`motion`  

The animation sequence to perform.

## Return Value

A progress object that reports the progress during execution of the animation sequence.

## Discussion

This method moves the dock accessory along a predefined trajectory to convey a characteristic. Do this only if you disable system tracking.

Throws

DockKitError.notConnected if device isn’t connected, DockKitError.frameRateTooHigh if calling the method too frequently, or DockKitError.notSupported in macOS.

## See Also

### Performing animation

func setRegionOfInterest(CGRect) async throws

Sets the area in the video frame in which the dock accessory tracks a subject.

var regionOfInterest: CGRect

The area in the video frame in which the dock accessory tracks a subject.

enum Animation

Character animations that describe how to move the dock accessory.

