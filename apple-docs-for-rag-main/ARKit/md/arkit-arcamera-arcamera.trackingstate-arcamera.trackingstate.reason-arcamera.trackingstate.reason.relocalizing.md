

- ARKit
- ARCamera
- ARCamera.TrackingState
- ARCamera.TrackingState.Reason
-  ARCamera.TrackingState.Reason.relocalizing 

Case

# ARCamera.TrackingState.Reason.relocalizing

The AR session is attempting to resume after an interruption.

iOS 11.3+iPadOS 11.3+

``` source
case relocalizing
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

ARKit cannot track device position or orientation when the session has been interrupted (for example, by dismissing the view hosting an AR session or switching to another app). When resuming the session after an interruption, the world coordinate system (used for placing anchors) likely no longer match the device’s real-world environment.

If your session or view delegate implements the sessionShouldAttemptRelocalization(_:) method and returns true, ARKit attempts to reconcile pre- and post-interruption world tracking state. During this process, called *relocalization*, world tracking quality is ARCamera.TrackingState.limited(_:), with a resaon value of ARCamera.TrackingState.Reason.relocalizing, indicating that hit tests and anchor placement are less accurate.

If successful, relocalization ends after a short time, tracking quality returns to the ARCamera.TrackingState.normal state, and the world coordinate system and anchor positions reflect their state before the interruption.

For relocalization to succeed, the device must be returned to a position and orientation approximately near where it was when the session was interrupted. If these conditions never occur (or cannot occur; for example, if the device has moved to an entirely different environment), the session will remain in the ARCamera.TrackingState.Reason.relocalizing state indefinitely.

Important

When in the ARCamera.TrackingState.Reason.relocalizing state, offer the user a way out in case relocalization never succeeds. For example, offer a button for resetting the session, which appears after the relocalizing state has remained for a fixed amount of time.

## See Also

### Inhibitors of Tracking Quality

case initializing

The AR session has not gathered enough camera or motion data to provide tracking information.

case excessiveMotion

The device is moving too fast for accurate image-based position tracking.

case insufficientFeatures

The scene visible to the camera doesn’t contain enough distinguishable features for image-based position tracking.

