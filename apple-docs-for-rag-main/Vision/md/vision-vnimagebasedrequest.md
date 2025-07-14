

- Vision
-  VNImageBasedRequest 

Class

# VNImageBasedRequest

The abstract superclass for image-analysis requests that focus on a specific part of an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNImageBasedRequest
```

## Overview

Other Vision request handlers that operate on still images inherit from this abstract base class. Don’t use it directly.

## Topics

### Configuring a Request

var regionOfInterest: CGRect

The region of the image in which Vision will perform the request.

## Relationships

### Inherits From

- VNRequest

### Inherited By

- VNCalculateImageAestheticsScoresRequest
- VNClassifyImageRequest
- VNCoreMLRequest
- VNDetectAnimalBodyPoseRequest
- VNDetectBarcodesRequest
- VNDetectContoursRequest
- VNDetectDocumentSegmentationRequest
- VNDetectFaceCaptureQualityRequest
- VNDetectFaceLandmarksRequest
- VNDetectFaceRectanglesRequest
- VNDetectHorizonRequest
- VNDetectHumanBodyPoseRequest
- VNDetectHumanHandPoseRequest
- VNDetectHumanRectanglesRequest
- VNDetectRectanglesRequest
- VNDetectTextRectanglesRequest
- VNGenerateAttentionBasedSaliencyImageRequest
- VNGenerateForegroundInstanceMaskRequest
- VNGenerateImageFeaturePrintRequest
- VNGenerateObjectnessBasedSaliencyImageRequest
- VNGeneratePersonInstanceMaskRequest
- VNRecognizeAnimalsRequest
- VNRecognizeTextRequest
- VNStatefulRequest
- VNTargetedImageRequest
- VNTrackingRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Still-image analysis

Detecting Objects in Still Images

Locate and demarcate rectangles, faces, barcodes, and text in images using the Vision framework.

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

Analyzing Image Similarity with Feature Print

Generate a feature print to compute distance between images.

class VNRequest

The abstract superclass for analysis requests.

class VNClassifyImageRequest

A request to classify an image.

class VNGenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

class VNObservation

The abstract superclass for analysis results.

