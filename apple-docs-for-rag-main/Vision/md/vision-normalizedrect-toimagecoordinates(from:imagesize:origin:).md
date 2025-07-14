

- Vision
- NormalizedRect
-  toImageCoordinates(from:imageSize:origin:) 

Instance Method

# toImageCoordinates(from:imageSize:origin:)

Converts a rectangle normalized to a region within an image into full image coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func toImageCoordinates(
    from regionOfInterest: NormalizedRect,
    imageSize: CGSize,
    origin: CoordinateOrigin = .lowerLeft
) -> CGRect
```

## Parameters 

`regionOfInterest`  

The region within an image you normalized the rect to.

`imageSize`  

The size of the image.

`origin`  

The origin.

## See Also

### Converting rectangles

func toImageCoordinates(CGSize, origin: CoordinateOrigin) -> CGRect

Converts a rectangle in normalized coordinates into image coordinates.

