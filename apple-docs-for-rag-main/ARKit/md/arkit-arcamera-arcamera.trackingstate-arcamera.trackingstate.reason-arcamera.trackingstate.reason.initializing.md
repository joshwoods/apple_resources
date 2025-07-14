

- ARKit
- ARCamera
- ARCamera.TrackingState
- ARCamera.TrackingState.Reason
-  ARCamera.TrackingState.Reason.initializing 

Case

# ARCamera.TrackingState.Reason.initializing

The AR session has not gathered enough camera or motion data to provide tracking information.

iOS 11.0+iPadOS 11.0+

``` source
case initializing
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

This value occurs temporarily after starting a new AR session or changing configurations.

## See Also

### Inhibitors of Tracking Quality

case relocalizing

The AR session is attempting to resume after an interruption.

case excessiveMotion

The device is moving too fast for accurate image-based position tracking.

case insufficientFeatures

The scene visible to the camera doesn’t contain enough distinguishable features for image-based position tracking.

