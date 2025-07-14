

- Vision
-  VNTextObservation 

Class

# VNTextObservation

Information about regions of text that an image-analysis request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNTextObservation
```

## Overview

This type of observation results from a VNDetectTextRectanglesRequest. It expresses the location of each detected character by its bounding box.

## Topics

### Finding Individual Characters

var characterBoxes: [VNRectangleObservation]?

An array of detected individual character bounding boxes.

## Relationships

### Inherits From

- VNRectangleObservation

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

### Text detection

class VNDetectTextRectanglesRequest

An image-analysis request that finds regions of visible text in an image.

