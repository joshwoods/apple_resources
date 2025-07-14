

- Vision
-  VNStatefulRequest 

Class

# VNStatefulRequest

An abstract request type that builds evidence of a condition over time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNStatefulRequest
```

## Topics

### Initializing a Request

init(frameAnalysisSpacing: CMTime, completionHandler: VNRequestCompletionHandler?)

Initializes a video-based request.

### Configuring the Request

var minimumLatencyFrameCount: Int

The minimum number of frames a request processes before reporting an observation.

var frameAnalysisSpacing: CMTime

A time value that indicates the interval between analysis operations.

## Relationships

### Inherits From

- VNImageBasedRequest

### Inherited By

- VNDetectHumanBodyPose3DRequest
- VNDetectTrajectoriesRequest
- VNGeneratePersonSegmentationRequest
- VNTrackHomographicImageRegistrationRequest
- VNTrackOpticalFlowRequest
- VNTrackTranslationalImageRegistrationRequest

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

class VNGeneratePersonSegmentationRequest

An object that produces a matte image for a person it finds in the input image.

class VNGeneratePersonInstanceMaskRequest

An object that produces a mask of individual people it finds in the input image.

class VNDetectDocumentSegmentationRequest

An object that detects rectangular regions that contain text in the input image.

class VNSequenceRequestHandler

An object that processes image-analysis requests for each frame in a sequence.

