

- ARKit
- ARCamera
- ARCamera.TrackingState
-  ARCamera.TrackingState.limited(\_:) 

Case

# ARCamera.TrackingState.limited(\_:)

Tracking is available, but the quality of results is questionable.

iOS 11.0+iPadOS 11.0+

``` source
case limited(ARCamera.TrackingState.Reason)
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

In this state, the positions and transforms of anchors in the scene (especially detected planes) may not be accurate or consistent from one captured frame to the next.

See the associated ARCamera.TrackingState.Reason value for information you can present to the user for improving tracking quality.

## See Also

### Determining the camera tracking status

case notAvailable

Camera position tracking is not available.

enum Reason

Causes of limited position-tracking quality.

case normal

Camera position tracking is providing optimal results.

