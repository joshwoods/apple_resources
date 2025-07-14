

- Vision
- NormalizedPoint
-  init(imagePoint:in:normalizedTo:) 

Initializer

# init(imagePoint:in:normalizedTo:)

Creates a point normalized to a region of interest within an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    imagePoint: CGPoint,
    in imageSize: CGSize,
    normalizedTo regionOfInterest: NormalizedRect
)
```

## Parameters 

`imagePoint`  

A point in the image coordinate space.

`imageSize`  

The size of the image.

`regionOfInterest`  

The region within the image to normalize the point to.

## See Also

### Creating a normalized point

init(x: CGFloat, y: CGFloat)

Creates a point object with the specified coordinates.

init(normalizedPoint: CGPoint)

Creates a point object from the specified Core Graphics point.

init(imagePoint: CGPoint, in: CGSize)

Creates a normalized point from a point in an image coordinate space.

static var zero: NormalizedPoint

A point object that represents the origin.

