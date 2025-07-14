

- ARKit
- ARCamera
- ARCamera.TrackingState
-  ARCamera.TrackingState.Reason 

Enumeration

# ARCamera.TrackingState.Reason

Causes of limited position-tracking quality.

iOS 11.0+iPadOS 11.0+

``` source
enum Reason
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Topics

### Inhibitors of Tracking Quality

case initializing

The AR session has not gathered enough camera or motion data to provide tracking information.

case relocalizing

The AR session is attempting to resume after an interruption.

case excessiveMotion

The device is moving too fast for accurate image-based position tracking.

case insufficientFeatures

The scene visible to the camera doesn’t contain enough distinguishable features for image-based position tracking.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Determining the camera tracking status

case notAvailable

Camera position tracking is not available.

case limited(ARCamera.TrackingState.Reason)

Tracking is available, but the quality of results is questionable.

case normal

Camera position tracking is providing optimal results.

