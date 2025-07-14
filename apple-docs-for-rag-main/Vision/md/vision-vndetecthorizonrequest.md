

- Vision
-  VNDetectHorizonRequest 

Class

# VNDetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectHorizonRequest
```

## Topics

### Accessing the Results

var results: [VNHorizonObservation]?

The results of the horizon detection request.

### Identifying Request Revisions

let VNDetectHorizonRequestRevision1: Int

A constant for specifying revision 1 of the horizon detection request.

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

### Horizon detection

class VNHorizonObservation

The horizon angle information that an image-analysis request detects.

