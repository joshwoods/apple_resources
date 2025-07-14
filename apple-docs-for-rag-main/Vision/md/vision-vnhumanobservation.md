

- Vision
-  VNHumanObservation 

Class

# VNHumanObservation

An object that represents a person that the request detects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class VNHumanObservation
```

## Topics

### Inspecting the Observation

var upperBodyOnly: Bool

A Boolean value that indicates whether the observation represents an upper-body or full-body rectangle.

## Relationships

### Inherits From

- VNDetectedObjectObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

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

class VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

