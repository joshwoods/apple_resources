

- Vision
-  VNDetectHumanRectanglesRequest 

Class

# VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNDetectHumanRectanglesRequest
```

## Topics

### Configuring the Request

var upperBodyOnly: Bool

A Boolean value that indicates whether the request requires detecting a full body or upper body only to produce a result.

### Accessing the Results

var results: [VNHumanObservation]?

The results of the request to find rectangular regions that contain people in an image.

### Identifying Request Revisions

let VNDetectHumanRectanglesRequestRevision2: Int

A constant for specifying revision 2 of the human rectangles detection request.

let VNDetectHumanRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the human rectangles detection request.

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

class VNDetectFaceRectanglesRequest

A request that finds faces within an image.

class VNHumanObservation

An object that represents a person that the request detects.

