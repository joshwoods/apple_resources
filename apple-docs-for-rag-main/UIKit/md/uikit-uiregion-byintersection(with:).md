

- UIKit
- UIRegion
-  byIntersection(with:) 

Instance Method

# byIntersection(with:)

Returns a new region containing only the area occupied by both the specified region and current region.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func byIntersection(with region: UIRegion) -> Self
```

## Parameters 

`region`  

The region to be intersected with the current region.

## Return Value

A new region that contains only the points that are in both the current region and the shape specified by the `region` parameter.

## See Also

### Creating complex regions

func inverse() -> Self

Returns a new region that’s the mathematical inverse of the current region.

func byDifference(from: UIRegion) -> Self

Returns a new region created by subtracting the specified region from the current region.

func byUnion(with: UIRegion) -> Self

Returns a new region containing the combined areas of the specified region and the current region.

