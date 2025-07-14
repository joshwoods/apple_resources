

- Vision
- NormalizedPoint
-  toImageCoordinates(\_:origin:) 

Instance Method

# toImageCoordinates(\_:origin:)

Converts a point in normalized coordinates into image coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func toImageCoordinates(
    _ imageSize: CGSize,
    origin: CoordinateOrigin = .lowerLeft
) -> CGPoint
```

## Parameters 

`imageSize`  

The size of the image.

`origin`  

The origin.

## See Also

### Converting points

func toImageCoordinates(from: NormalizedRect, imageSize: CGSize, origin: CoordinateOrigin) -> CGPoint

Converts a point normalized to a region within an image into full image coordinates.

