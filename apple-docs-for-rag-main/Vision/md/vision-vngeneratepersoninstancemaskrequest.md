

- Vision
-  VNGeneratePersonInstanceMaskRequest 

Class

# VNGeneratePersonInstanceMaskRequest

An object that produces a mask of individual people it finds in the input image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNGeneratePersonInstanceMaskRequest
```

## Topics

### Accessing the Results

var results: [VNInstanceMaskObservation]?

The results of the instance mask request.

### Identifying Request Revisions

let VNGeneratePersonInstanceMaskRequestRevision1: Int

A constant for specifying revision 1 of the person instance mask request.

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

### Image sequence analysis

Applying Matte Effects to People in Images and Video

Generate image masks for people automatically by using semantic person-segmentation.

Detecting Human Actions in a Live Video Feed

Identify body movements by sending a person’s pose data from a series of video frames to an action-classification model.

Segmenting and colorizing individuals from a surrounding scene

Use the Vision framework to isolate and apply colors to people in an image.

class VNStatefulRequest

An abstract request type that builds evidence of a condition over time.

class VNGeneratePersonSegmentationRequest

An object that produces a matte image for a person it finds in the input image.

class VNDetectDocumentSegmentationRequest

An object that detects rectangular regions that contain text in the input image.

class VNSequenceRequestHandler

An object that processes image-analysis requests for each frame in a sequence.

