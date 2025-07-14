

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Classification
- ARPlaneAnchor.Classification.Status
-  ARPlaneAnchor.Classification.Status.undetermined 

Case

# ARPlaneAnchor.Classification.Status.undetermined

ARKit has not yet produced a classification for the plane anchor.

iOS 12.0+iPadOS 12.0+

``` source
case undetermined
```

## Discussion

This status occurs when ARKit is still in the process of plane classification. To be notified when ARKit produces a classification, observe the same plane anchor in a later frame (for example, in the session(_:didUpdate:) or renderer(_:didUpdate:for:) delegate method).

## See Also

### Classification Status

case notAvailable

ARKit cannot currently provide plane classification information.

case unknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

