

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Classification
- ARPlaneAnchor.Classification.Status
-  ARPlaneAnchor.Classification.Status.unknown 

Case

# ARPlaneAnchor.Classification.Status.unknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

iOS 12.0+iPadOS 12.0+

``` source
case unknown
```

## Discussion

ARKit attempts to classify detected planes using a finite set of common categories. However, a detected plane may not be a real object fitting any of those categories, or the plane classification process may not be able to recognize it. In such cases, the plane anchor’s classification is ARPlaneAnchor.Classification.none(_:) with an associated value of ARPlaneAnchor.Classification.Status.unknown.

## See Also

### Classification Status

case notAvailable

ARKit cannot currently provide plane classification information.

case undetermined

ARKit has not yet produced a classification for the plane anchor.

