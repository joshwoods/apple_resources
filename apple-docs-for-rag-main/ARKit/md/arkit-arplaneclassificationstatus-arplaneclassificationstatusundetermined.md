

- ARKit
- ARPlaneClassificationStatus
-  ARPlaneClassificationStatusUndetermined 

Enumeration Case

# ARPlaneClassificationStatusUndetermined

ARKit has not yet produced a classification for the plane anchor.

``` source
ARPlaneClassificationStatusUndetermined
```

## Discussion

This status occurs when ARKit is still in the process of plane classification. To be notified when ARKit produces a classification, observe the same plane anchor in a later frame (for example, in the session(_:didUpdate:) or renderer(_:didUpdate:for:) delegate method).

## See Also

### Classification Status

ARPlaneClassificationStatusNotAvailable

ARKit cannot currently provide plane classification information.

ARPlaneClassificationStatusUnknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

ARPlaneClassificationStatusKnown

ARKit has completed its classfication process for the plane anchor.

