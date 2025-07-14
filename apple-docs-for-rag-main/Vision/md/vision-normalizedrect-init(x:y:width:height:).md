

- Vision
- NormalizedRect
-  init(x:y:width:height:) 

Initializer

# init(x:y:width:height:)

Creates a rectangle with the specified coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    x: CGFloat,
    y: CGFloat,
    width: CGFloat,
    height: CGFloat
)
```

## Parameters 

`x`  

The x-coordinate of the rectangle’s lower-left corner.

`y`  

The y-coordinate of the rectangle’s lower-left corner.

`width`  

The width of the rectangle.

`height`  

The hight of the rectangle.

## See Also

### Creating a normalized rectangle

init(imageRect: CGRect, in: CGSize)

Creates a normalized rectangle from a rectangle in an image coordinate space.

init(imageRect: CGRect, in: CGSize, normalizedTo: NormalizedRect)

Creates a rectangle normalized to a region of interest in an image from a rectangle in an image coordinate space.

init(normalizedRect: CGRect)

Creates a rectangle from the specified Core Graphics rectangle.

static var fullImage: NormalizedRect

A normalized rectangle with an origin at zero and a width and height of one.

