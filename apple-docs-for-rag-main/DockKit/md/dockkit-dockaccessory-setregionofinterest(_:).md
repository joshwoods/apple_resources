

- DockKit
- DockAccessory
-  setRegionOfInterest(\_:) 

Instance Method

# setRegionOfInterest(\_:)

Sets the area in the video frame in which the dock accessory tracks a subject.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func setRegionOfInterest(_ region: CGRect) async throws
```

## Parameters 

`region`  

The area in the video frame in which the dock accessory tracks a subject.

## Discussion

The region of interest is an limited area within the video frame that DockKit tracks a subject in. The default value is `(0,0,1,1)`, which indicates that the whole frame is of interest.

If you disable system tracking, this configuration change applies to any custom tracking for this dock accessory. The configuration applies to any camera stream the app has open if system tracking is enabled.

The region of interest doesn’t persist; it resets to the entire video frame any time an app exits, backgrounds, or stops tracking.

Throws

DockKitError.notConnected if device isn’t connected, or DockKitError.notSupported if called on macOS.

## See Also

### Performing animation

func animate(motion: DockAccessory.Animation) async throws -> Progress

Starts an animation sequence.

var regionOfInterest: CGRect

The area in the video frame in which the dock accessory tracks a subject.

enum Animation

Character animations that describe how to move the dock accessory.

