

- ARKit
- ARCamera
-  ARCamera.TrackingState 

Enumeration

# ARCamera.TrackingState

Values for position tracking quality, with possible causes when tracking quality is limited.

iOS 11.0+iPadOS 11.0+

``` source
@frozen
enum TrackingState
```

## Topics

### Determining the camera tracking status

case notAvailable

Camera position tracking is not available.

case limited(ARCamera.TrackingState.Reason)

Tracking is available, but the quality of results is questionable.

enum Reason

Causes of limited position-tracking quality.

case normal

Camera position tracking is providing optimal results.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Handling Tracking Status

var trackingState: ARCamera.TrackingState

The general quality of position tracking available when the camera captured a frame.

