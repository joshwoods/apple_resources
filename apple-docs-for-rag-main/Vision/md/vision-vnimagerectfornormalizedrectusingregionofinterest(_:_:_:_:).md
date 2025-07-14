

- Vision
-  VNImageRectForNormalizedRectUsingRegionOfInterest(\_:\_:\_:\_:) 

Function

# VNImageRectForNormalizedRectUsingRegionOfInterest(\_:\_:\_:\_:)

Projects a rectangle from a region of interest within the normalized coordinates into image coordinates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func VNImageRectForNormalizedRectUsingRegionOfInterest(
    _ normalizedRect: CGRect,
    _ imageWidth: Int,
    _ imageHeight: Int,
    _ roi: CGRect
) -> CGRect
```

## Parameters 

`normalizedRect`  

The rectangle in normalized coordinates.

`imageWidth`  

The width of the image.

`imageHeight`  

The height of the image.

`roi`  

The region of interest within the normalized-coordinate space.

## Return Value

A rectangle in the image-coordinate space.

## See Also

### Coordinate conversion

func VNImagePointForNormalizedPoint(CGPoint, Int, Int) -> CGPoint

Projects a point in normalized coordinates into image coordinates.

func VNNormalizedPointForImagePoint(CGPoint, Int, Int) -> CGPoint

Projects a point from image coordinates into normalized coordinates.

func VNImagePointForNormalizedPointUsingRegionOfInterest(CGPoint, Int, Int, CGRect) -> CGPoint

Projects a point from a region of interest within the normalized coordinates into image coordinates.

func VNNormalizedPointForImagePointUsingRegionOfInterest(CGPoint, Int, Int, CGRect) -> CGPoint

Projects a point from a region of interest within the image coordinates into normalized coordinates.

func VNImageRectForNormalizedRect(CGRect, Int, Int) -> CGRect

Projects a rectangle from normalized coordinates into image coordinates.

func VNNormalizedRectForImageRect(CGRect, Int, Int) -> CGRect

Projects a rectangle from image coordinates into normalized coordinates.

func VNNormalizedRectForImageRectUsingRegionOfInterest(CGRect, Int, Int, CGRect) -> CGRect

Projects a rectangle from a region of interest within the image coordinates space into normalized coordinates.

let VNNormalizedIdentityRect: CGRect

A normalized identity rectangle with an origin of zero and unit length and width.

func VNNormalizedRectIsIdentityRect(CGRect) -> Bool

Returns a Boolean value that indicates whether the rectangle has an origin of zero and unit length and width.

func VNImagePointForFaceLandmarkPoint(vector_float2, CGRect, Int, Int) -> CGPoint

Returns the image coordinates of a specified face landmark point.

func VNNormalizedFaceBoundingBoxPointForLandmarkPoint(vector_float2, CGRect, Int, Int) -> CGPoint

Returns the coordinates of a specified face landmark point, in bounding box coordinates.

