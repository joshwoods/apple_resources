

- ARKit
- ARCamera
- ARCamera.TrackingState
- ARCamera.TrackingState.Reason
-  ARCamera.TrackingState.Reason.excessiveMotion 

Case

# ARCamera.TrackingState.Reason.excessiveMotion

The device is moving too fast for accurate image-based position tracking.

iOS 11.0+iPadOS 11.0+

``` source
case excessiveMotion
```

## See Also

### Inhibitors of Tracking Quality

case initializing

The AR session has not gathered enough camera or motion data to provide tracking information.

case relocalizing

The AR session is attempting to resume after an interruption.

case insufficientFeatures

The scene visible to the camera doesn’t contain enough distinguishable features for image-based position tracking.

