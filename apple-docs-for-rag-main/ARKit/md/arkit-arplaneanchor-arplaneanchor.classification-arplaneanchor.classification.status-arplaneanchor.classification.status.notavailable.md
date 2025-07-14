

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Classification
- ARPlaneAnchor.Classification.Status
-  ARPlaneAnchor.Classification.Status.notAvailable 

Case

# ARPlaneAnchor.Classification.Status.notAvailable

ARKit cannot currently provide plane classification information.

iOS 12.0+iPadOS 12.0+

``` source
case notAvailable
```

## Discussion

Plane classification is available only on iPhone XS and iPhone XS Max devices. On other devices, all plane anchors always indicate a classification status of ARPlaneAnchor.Classification.Status.notAvailable.

A classification status of ARPlaneAnchor.Classification.Status.notAvailable can also occur if the plane classification process is temporarily unavilable.

## See Also

### Classification Status

case undetermined

ARKit has not yet produced a classification for the plane anchor.

case unknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

