

- RealityKit
- BoundingBox
-  empty 

Type Property

# empty

An empty bounding box.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static let empty: BoundingBox
```

## Discussion

An empty bounding box is defined with min set to positive infinity and max set to negative infinity.

Note

An empty bounding box where min is greater than max is different from a bounding box of size 0, where min is equal to max. The former defines empty space without a position. The latter describes an object of size 0 at a certain position in space.

## See Also

### Getting an empty box

var isEmpty: Bool

A Boolean that indicates whether the bounding box is empty.

