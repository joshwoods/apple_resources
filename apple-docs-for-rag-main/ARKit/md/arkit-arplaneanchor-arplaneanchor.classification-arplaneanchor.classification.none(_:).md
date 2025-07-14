

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Classification
-  ARPlaneAnchor.Classification.none(\_:) 

Case

# ARPlaneAnchor.Classification.none(\_:)

No classification is available for the plane anchor.

iOS 12.0+iPadOS 12.0+

``` source
case none(ARPlaneAnchor.Classification.Status)
```

## Discussion

Plane classification can take longer than plane detection, and ARKit reports classifications only for planes where it has a high confidence in the result. See the associated ARPlaneAnchor.Classification.Status value for the reason a plane anchor reports no classification.

## See Also

### Missing Classification Status

enum Status

Reasons ARKit is unable to classify a plane.

