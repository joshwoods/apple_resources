

- ARKit
- ARTrackingState
-  ARTrackingStateLimited 

Enumeration Case

# ARTrackingStateLimited

Tracking is available, but the quality of results is questionable.

``` source
ARTrackingStateLimited
```

## Discussion

In this state, the positions and transforms of anchors in the scene (especially detected planes) may not be accurate or consistent from one captured frame to the next.

See the associated ARTrackingStateReason value for information you can present to the user for improving tracking quality.

## See Also

### Tracking States

ARTrackingStateNotAvailable

Camera position tracking is not available.

ARTrackingStateNormal

Camera position tracking is providing optimal results.

