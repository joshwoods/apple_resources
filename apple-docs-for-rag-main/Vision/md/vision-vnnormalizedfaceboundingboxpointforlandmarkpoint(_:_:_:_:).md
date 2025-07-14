

- Vision
-  VNNormalizedFaceBoundingBoxPointForLandmarkPoint(\_:\_:\_:\_:) 

Function

# VNNormalizedFaceBoundingBoxPointForLandmarkPoint(\_:\_:\_:\_:)

Returns the coordinates of a specified face landmark point, in bounding box coordinates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func VNNormalizedFaceBoundingBoxPointForLandmarkPoint(
    _ faceLandmarkPoint: vector_float2,
    _ faceBoundingBox: CGRect,
    _ imageWidth: Int,
    _ imageHeight: Int
) -> CGPoint
```

## Parameters 

`faceLandmarkPoint`  

The location of the face landmark, as returned from a VNFaceLandmarkRegion2D instance.

`faceBoundingBox`  

The normalized bounding box rect around the face, as obtained from a VNFaceObservation instance.

`imageWidth`  

The width of the image from which the VNFaceObservation instance was generated.

`imageHeight`  

The height of the image from which the VNFaceObservation instance was generated.

## Return Value

The input point projected into normalized bounding box coordinates.

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

