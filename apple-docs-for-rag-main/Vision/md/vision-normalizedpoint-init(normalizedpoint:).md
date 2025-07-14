

- Vision
- NormalizedPoint
-  init(normalizedPoint:) 

Initializer

# init(normalizedPoint:)

Creates a point object from the specified Core Graphics point.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(normalizedPoint: CGPoint)
```

## Parameters 

`normalizedPoint`  

The Core Graphics point.

## See Also

### Creating a normalized point

init(x: CGFloat, y: CGFloat)

Creates a point object with the specified coordinates.

init(imagePoint: CGPoint, in: CGSize)

Creates a normalized point from a point in an image coordinate space.

init(imagePoint: CGPoint, in: CGSize, normalizedTo: NormalizedRect)

Creates a point normalized to a region of interest within an image.

static var zero: NormalizedPoint

A point object that represents the origin.

