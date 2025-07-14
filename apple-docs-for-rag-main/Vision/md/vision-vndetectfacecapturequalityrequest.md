

- Vision
-  VNDetectFaceCaptureQualityRequest 

Class

# VNDetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNDetectFaceCaptureQualityRequest
```

## Overview

This request produces or updates a VNFaceObservation object’s property faceCaptureQuality with a floating-point value. The value ranges from `0` to `1`. Faces with quality closer to `1` are better lit, sharper, and more centrally positioned than faces with quality closer to `0`.

If you don’t execute the request, or the request fails, the property faceCaptureQuality is nil.

## Topics

### Accessing the Results

var results: [VNFaceObservation]?

The results of the face-capture quality request.

class VNFaceObservation

Face or facial-feature information that an image analysis request detects.

### Identifying Request Revisions

let VNDetectFaceCaptureQualityRequestRevision2: Int

Revision 2 of the request algorithm.

let VNDetectFaceCaptureQualityRequestRevision1: Int

A constant for specifying revision 1 of the face capture detection request.

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
- VNFaceObservationAccepting

## See Also

### Face and body detection

Selecting a selfie based on capture quality

Compare face-capture quality in a set of images by using Vision.

class VNDetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

class VNDetectFaceRectanglesRequest

A request that finds faces within an image.

class VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

class VNHumanObservation

An object that represents a person that the request detects.

