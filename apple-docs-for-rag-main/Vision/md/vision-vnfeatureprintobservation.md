

- Vision
-  VNFeaturePrintObservation 

Class

# VNFeaturePrintObservation

An observation that provides the recognized feature print.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNFeaturePrintObservation
```

## Topics

### Fetching Feature Print Data

var data: Data

The feature print data.

var elementCount: Int

The total number of elements in the data.

### Determining Types of Feature Prints

var elementType: VNElementType

The type of each element in the data.

enum VNElementType

An enumeration of the type of element in feature print data.

func VNElementTypeSize(VNElementType) -> Int

Returns the size of a feature print element.

### Computing Distance Between Features

func computeDistance(UnsafeMutablePointer&lt;Float>, to: VNFeaturePrintObservation) throws

Computes the distance between two feature print observations.

## Relationships

### Inherits From

- VNObservation

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

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

class VNObservation

The abstract superclass for analysis results.

