

- SpriteKit
- SKRegion
-  init(size:) 

Initializer

# init(size:)

Initializes a new region with a rectangular area.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(size: CGSize)
```

## Parameters 

`size`  

The size of the rectangle in points.

## Return Value

A newly initialized region. The region is rectangular and centered on the origin.

## See Also

### Creating and Initializing Region Objects

class func infinite() -> Self

Returns a region that defines a region that includes all points.

init(radius: Float)

Initializes a new region with a circular area.

init(path: CGPath)

Initializes a new region using a Core Graphics path.

func inverse() -> Self

Returns a new region that is the mathematical inverse of an existing region.

func byDifference(from: SKRegion) -> Self

Returns a new region created by subtracting the contents of another region from this region.

func byIntersection(with: SKRegion) -> Self

Returns a new region created by intersecting the contents of this region with another region.

func byUnion(with: SKRegion) -> Self

Returns a new region created by combining the contents of this region with another region.

