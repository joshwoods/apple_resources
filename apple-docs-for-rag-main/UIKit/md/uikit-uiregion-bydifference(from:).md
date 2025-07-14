

- UIKit
- UIRegion
-  byDifference(from:) 

Instance Method

# byDifference(from:)

Returns a new region created by subtracting the specified region from the current region.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func byDifference(from region: UIRegion) -> Self
```

## Parameters 

`region`  

The region to be subtracted from the current region.

## Return Value

A new region that contains the points that are in the current region and not in the area defined by the `region` parameter.

## See Also

### Creating complex regions

func inverse() -> Self

Returns a new region that’s the mathematical inverse of the current region.

func byIntersection(with: UIRegion) -> Self

Returns a new region containing only the area occupied by both the specified region and current region.

func byUnion(with: UIRegion) -> Self

Returns a new region containing the combined areas of the specified region and the current region.

