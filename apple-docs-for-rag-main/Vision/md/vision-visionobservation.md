

- Vision
-  VisionObservation 

Protocol

# VisionObservation

A type for objects produced by image-analysis requests.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol VisionObservation : CustomStringConvertible, Decodable, Encodable, Hashable, Sendable
```

## Topics

### Inspecting an observation

var uuid: UUID

A unique alphanumeric value that the framework assigns the observation.

**Required**

var confidence: Float

The level of confidence in the observation’s accuracy.

**Required**

var description: String

A textual representation of this instance.

**Required**

var originatingRequestDescriptor: RequestDescriptor?

The descriptor of the request that produces the observation.

**Required**

enum RequestDescriptor

A type that describes the request and revision combination.

var timeRange: CMTimeRange?

The time range of the reported observation.

**Required**

### Hashing the observation

func hash(into: inout Hasher)

Hashes the essential components of the value by passing them into the hasher.

**Required** Default implementation provided.

### Default Implementations

Hashable Implementations

## Relationships

### Inherits From

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

### Conforming Types

- AnimalBodyPoseObservation
- BarcodeObservation
- ClassificationObservation
- ContoursObservation
- CoreMLFeatureValueObservation
- DetectedDocumentObservation
- DetectedObjectObservation
- FaceObservation
- FeaturePrintObservation
- HorizonObservation
- HumanBodyPose3DObservation
- HumanBodyPoseObservation
- HumanHandPoseObservation
- HumanObservation
- ImageAestheticsScoresObservation
- ImageHomographicAlignmentObservation
- ImageTranslationAlignmentObservation
- InstanceMaskObservation
- OpticalFlowObservation
- PixelBufferObservation
- RecognizedObjectObservation
- RecognizedTextObservation
- RectangleObservation
- SaliencyImageObservation
- TextObservation
- TrajectoryObservation

## See Also

### Still-image analysis

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

struct ClassifyImageRequest

A request to classify an image.

protocol ImageProcessingRequest

A type for image-analysis requests that focus on a specific part of an image.

class ImageRequestHandler

An object that processes one or more image-analysis requests pertaining to a single image.

protocol VisionRequest

A type for image-analysis requests.

