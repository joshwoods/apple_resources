

- Vision
-  VNObservation 

Class

# VNObservation

The abstract superclass for analysis results.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNObservation
```

## Overview

Observations resulting from Vision image analysis requests inherit from this abstract base class. Don’t use this abstract superclass directly.

## Topics

### Tracking Observations

var uuid: UUID

A unique identifier assigned to the Vision observation.

### Evaluating Observations

var timeRange: CMTimeRange

The time range of the reported observation.

var confidence: VNConfidence

The level of confidence in the observation’s accuracy.

typealias VNConfidence

A type alias for the confidence value of an observation.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VNClassificationObservation
- VNContoursObservation
- VNCoreMLFeatureValueObservation
- VNDetectedObjectObservation
- VNFeaturePrintObservation
- VNHorizonObservation
- VNImageAestheticsScoresObservation
- VNImageAlignmentObservation
- VNInstanceMaskObservation
- VNPixelBufferObservation
- VNRecognizedPoints3DObservation
- VNRecognizedPointsObservation
- VNTrajectoryObservation

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

### Still-image analysis

Detecting Objects in Still Images

Locate and demarcate rectangles, faces, barcodes, and text in images using the Vision framework.

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

Analyzing Image Similarity with Feature Print

Generate a feature print to compute distance between images.

class VNRequest

The abstract superclass for analysis requests.

class VNImageBasedRequest

The abstract superclass for image-analysis requests that focus on a specific part of an image.

class VNClassifyImageRequest

A request to classify an image.

class VNGenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

