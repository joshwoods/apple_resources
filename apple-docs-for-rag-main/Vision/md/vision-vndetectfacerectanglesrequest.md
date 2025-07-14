

- Vision
-  VNDetectFaceRectanglesRequest 

Class

# VNDetectFaceRectanglesRequest

A request that finds faces within an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectFaceRectanglesRequest
```

## Overview

This request returns faces as rectangular bounding boxes with origin and size.

## Topics

### Accessing the Results

var results: [VNFaceObservation]?

The results of the face detection request.

class VNFaceObservation

Face or facial-feature information that an image analysis request detects.

### Identifying Request Revisions

let VNDetectFaceRectanglesRequestRevision3: Int

A constant for specifying revision 3 of the face rectangles detection request.

let VNDetectFaceRectanglesRequestRevision2: Int

A constant for specifying revision 2 of the face rectangles detection request.

let VNDetectFaceRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the face rectangles detection request.

Deprecated

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Face and body detection

Selecting a selfie based on capture quality

Compare face-capture quality in a set of images by using Vision.

class VNDetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

class VNDetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

class VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

class VNHumanObservation

An object that represents a person that the request detects.

