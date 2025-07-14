

- Vision
- VNFaceObservation
-  landmarks 

Instance Property

# landmarks

The facial features of the detected face.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var landmarks: VNFaceLandmarks2D? { get }
```

## Discussion

This value is `nil` for face observations produced by a VNDetectFaceRectanglesRequest analysis. Use the VNDetectFaceLandmarksRequest class to find facial features.

## See Also

### Identifying Landmarks

class VNFaceLandmarks2D

A collection of facial features that a request detects.

class VNFaceLandmarkRegion2D

2D geometry information for a specific facial feature.

class VNFaceLandmarks

The abstract superclass for containers of face landmark information.

class VNFaceLandmarkRegion

The abstract superclass for information about a specific face landmark.

