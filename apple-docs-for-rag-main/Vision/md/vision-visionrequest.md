

- Vision
-  VisionRequest 

Protocol

# VisionRequest

A type for image-analysis requests.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol VisionRequest : CustomStringConvertible, Hashable, Sendable
```

## Topics

### Getting the compute device

func computeDevice(for: ComputeStage) -> MLComputeDevice?

Returns the compute device for a compute stage.

**Required**

var supportedComputeStageDevices: [ComputeStage : [MLComputeDevice]]

The collection of compute devices per stage that a request supports.

**Required**

enum ComputeStage

Types that represent the compute stage.

### Setting the compute device

func setComputeDevice(MLComputeDevice?, for: ComputeStage)

Assigns a compute device for a compute stage.

**Required**

### Performing the request

associatedtype Result

An associated type that represents the result.

**Required**

enum VisionResult

The result the framework produces by performing a request.

### Instance Properties

var descriptor: RequestDescriptor

An enum that identifies the request and request revision.

**Required**

## Relationships

### Inherits From

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

### Inherited By

- ImageProcessingRequest
- StatefulRequest
- TargetedRequest

### Conforming Types

- CalculateImageAestheticsScoresRequest
- ClassifyImageRequest
- CoreMLRequest
- DetectAnimalBodyPoseRequest
- DetectBarcodesRequest
- DetectContoursRequest
- DetectDocumentSegmentationRequest
- DetectFaceCaptureQualityRequest
- DetectFaceLandmarksRequest
- DetectFaceRectanglesRequest
- DetectHorizonRequest
- DetectHumanBodyPose3DRequest
- DetectHumanBodyPoseRequest
- DetectHumanHandPoseRequest
- DetectHumanRectanglesRequest
- DetectRectanglesRequest
- DetectTextRectanglesRequest
- DetectTrajectoriesRequest
- GenerateAttentionBasedSaliencyImageRequest
- GenerateForegroundInstanceMaskRequest
- GenerateImageFeaturePrintRequest
- GenerateObjectnessBasedSaliencyImageRequest
- GeneratePersonInstanceMaskRequest
- GeneratePersonSegmentationRequest
- RecognizeAnimalsRequest
- RecognizeTextRequest
- TrackHomographicImageRegistrationRequest
- TrackObjectRequest
- TrackOpticalFlowRequest
- TrackRectangleRequest
- TrackTranslationalImageRegistrationRequest

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

protocol VisionObservation

A type for objects produced by image-analysis requests.

