

- Vision
-  VNDetectTextRectanglesRequest 

Class

# VNDetectTextRectanglesRequest

An image-analysis request that finds regions of visible text in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectTextRectanglesRequest
```

## Overview

This request returns detected text characters as rectangular bounding boxes with origin and size.

## Topics

### Configuring a Request

var reportCharacterBoxes: Bool

A Boolean value that indicates whether the request detects character bounding boxes.

### Accessing the Results

var results: [VNTextObservation]?

The results of the request to detect text rectangles.

### Identifying Request Revisions

let VNDetectTextRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the text rectangles detection request.

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

### Text detection

class VNTextObservation

Information about regions of text that an image-analysis request detects.

