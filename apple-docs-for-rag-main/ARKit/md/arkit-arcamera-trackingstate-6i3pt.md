

- ARKit
- ARCamera
-  trackingState 

Instance Property

# trackingState

The general quality of position tracking available when the camera captured a frame.

iOS 11.0+iPadOS 11.0+

``` source
var trackingState: ARCamera.TrackingState { get }
```

## Discussion

When this value is ARCamera.TrackingState.limited(_:), see the associated ARCamera.TrackingState.Reason value for a possible cause of low tracking quality.

## See Also

### Handling Tracking Status

enum TrackingState

Values for position tracking quality, with possible causes when tracking quality is limited.

