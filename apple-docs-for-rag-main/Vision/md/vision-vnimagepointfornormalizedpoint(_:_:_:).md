

- Vision
-  VNImagePointForNormalizedPoint(\_:\_:\_:) 

Function

# VNImagePointForNormalizedPoint(\_:\_:\_:)

Projects a point in normalized coordinates into image coordinates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func VNImagePointForNormalizedPoint(
    _ normalizedPoint: CGPoint,
    _ imageWidth: Int,
    _ imageHeight: Int
) -> CGPoint
```

## Parameters 

`normalizedPoint`  

The input point in normalized coordinate space.

`imageWidth`  

The width of the image into whose coordinate space you’re projecting the input point.

`imageHeight`  

The height of the image into whose coordinate space you’re projecting the input point.

## Return Value

The input point projected into image coordinates.

## Mentioned in 

Detecting Human Body Poses in Images

## Discussion

The resulting point in image coordinate space may have nonintegral (floating-point) coordinates.

## See Also

### Coordinate conversion

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

func VNImageRectForNormalizedRectUsingRegionOfInterest(CGRect, Int, Int, CGRect) -> CGRect

Projects a rectangle from a region of interest within the normalized coordinates into image coordinates.

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

