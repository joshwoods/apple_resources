

- Vision
- NormalizedRect
-  init(imageRect:in:) 

Initializer

# init(imageRect:in:)

Creates a normalized rectangle from a rectangle in an image coordinate space.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    imageRect: CGRect,
    in imageSize: CGSize
)
```

## Parameters 

`imageRect`  

A rectangle in the image coordinate space.

`imageSize`  

The size of the image.

## See Also

### Creating a normalized rectangle

init(x: CGFloat, y: CGFloat, width: CGFloat, height: CGFloat)

Creates a rectangle with the specified coordinates.

init(imageRect: CGRect, in: CGSize, normalizedTo: NormalizedRect)

Creates a rectangle normalized to a region of interest in an image from a rectangle in an image coordinate space.

init(normalizedRect: CGRect)

Creates a rectangle from the specified Core Graphics rectangle.

static var fullImage: NormalizedRect

A normalized rectangle with an origin at zero and a width and height of one.

