

- Vision
-  VNGenerateImageFeaturePrintRequest 

Class

# VNGenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNGenerateImageFeaturePrintRequest
```

## Overview

This request returns the feature print data it generates as an array of VNFeaturePrintObservation objects.

## Topics

### Scaling and Cropping Images

var imageCropAndScaleOption: VNImageCropAndScaleOption

An optional setting that tells the algorithm how to scale an input image before generating the feature print.

enum VNImageCropAndScaleOption

Options that define how Vision crops and scales an input-image.

### Accessing the Results

var results: [VNFeaturePrintObservation]?

The results of the feature print request.

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

### Identifying Request Revisions

let VNGenerateImageFeaturePrintRequestRevision1: Int

A constant for specifying the first revision of the feature-print request.

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

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

class VNObservation

The abstract superclass for analysis results.

