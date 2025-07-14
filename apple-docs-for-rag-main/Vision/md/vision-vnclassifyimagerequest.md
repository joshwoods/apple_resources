

- Vision
-  VNClassifyImageRequest 

Class

# VNClassifyImageRequest

A request to classify an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNClassifyImageRequest
```

## Overview

This type of request produces a collection of VNClassificationObservation objects that describe an image. Access the classifications through knownClassifications(forRevision:).

## Topics

### Accessing Results

func supportedIdentifiers() throws -> [String]

Returns the classification identifiers that the request supports in its current configuration.

var results: [VNClassificationObservation]?

The results of the image classification request.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class func knownClassifications(forRevision: Int) throws -> [VNClassificationObservation]

Requests the collection of classifications that the Vision framework recognizes.

Deprecated

### Specifying Algorithm Revision

let VNClassifyImageRequestRevision1: Int

A constant for specifying the first revision of the image-classification request.

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

class VNGenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

class VNObservation

The abstract superclass for analysis results.

