

- Vision
-  ImageProcessingRequest 

Protocol

# ImageProcessingRequest

A type for image-analysis requests that focus on a specific part of an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol ImageProcessingRequest : VisionRequest
```

## Topics

### Setting the region

var regionOfInterest: NormalizedRect

The region of the image where the framework performs the request.

**Required**

### Performing a request

func perform(on: URL, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on an image URL and produces observations.

**Required** Default implementations provided.

func perform(on: Data, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on image data and produces observations.

**Required** Default implementations provided.

func perform(on: CGImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Graphics image and produces observations.

**Required** Default implementations provided.

func perform(on: CVPixelBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a pixel buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CMSampleBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Media buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CIImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Image image and produces observations.

**Required** Default implementations provided.

## Relationships

### Inherits From

- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- VisionRequest

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

class ImageRequestHandler

An object that processes one or more image-analysis requests pertaining to a single image.

protocol VisionRequest

A type for image-analysis requests.

protocol VisionObservation

A type for objects produced by image-analysis requests.

