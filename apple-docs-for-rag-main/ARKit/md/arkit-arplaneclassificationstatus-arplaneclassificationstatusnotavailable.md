

- ARKit
- ARPlaneClassificationStatus
-  ARPlaneClassificationStatusNotAvailable 

Enumeration Case

# ARPlaneClassificationStatusNotAvailable

ARKit cannot currently provide plane classification information.

``` source
ARPlaneClassificationStatusNotAvailable
```

## Discussion

Plane classification is available only on iPhone XS, iPhone XS Max, and iPhone XR. On other devices, all plane anchors always indicate a classification status of ARPlaneClassificationStatusNotAvailable.

A classification status of ARPlaneClassificationStatusNotAvailable can also occur if the plane classification process is temporarily unavilable.

## See Also

### Classification Status

ARPlaneClassificationStatusUndetermined

ARKit has not yet produced a classification for the plane anchor.

ARPlaneClassificationStatusUnknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

ARPlaneClassificationStatusKnown

ARKit has completed its classfication process for the plane anchor.

