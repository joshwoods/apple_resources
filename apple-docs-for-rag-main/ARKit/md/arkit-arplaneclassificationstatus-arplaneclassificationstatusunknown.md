

- ARKit
- ARPlaneClassificationStatus
-  ARPlaneClassificationStatusUnknown 

Enumeration Case

# ARPlaneClassificationStatusUnknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

``` source
ARPlaneClassificationStatusUnknown
```

## Discussion

ARKit attempts to classify detected planes using a finite set of common categories. However, a detected plane may not be a real object fitting any of those categories, or the plane classification process may not be able to recognize it. In such cases, the plane anchor’s classification is ARPlaneClassificationNone and its classificationStatus is ARPlaneClassificationStatusUnknown.

## See Also

### Classification Status

ARPlaneClassificationStatusNotAvailable

ARKit cannot currently provide plane classification information.

ARPlaneClassificationStatusUndetermined

ARKit has not yet produced a classification for the plane anchor.

ARPlaneClassificationStatusKnown

ARKit has completed its classfication process for the plane anchor.

