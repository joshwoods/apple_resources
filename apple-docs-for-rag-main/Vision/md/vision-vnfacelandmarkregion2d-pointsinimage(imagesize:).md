

- Vision
- VNFaceLandmarkRegion2D
-  pointsInImage(imageSize:) 

Instance Method

# pointsInImage(imageSize:)

Returns an array containing landmark points in the coordinate space of the specified image size.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@nonobjc
func pointsInImage(imageSize: CGSize) -> [CGPoint]
```

## Parameters 

`imageSize`  

The pixel dimensions of the image in which to present landmark points.

## Return Value

An array containing a CGPoint for each landmark the system detects in the image, expressed in the coordinate space of the specified image size.

