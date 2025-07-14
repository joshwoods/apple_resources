

- Vision
-  VNImageAestheticsScoresObservation 

Class

# VNImageAestheticsScoresObservation

An object that represents the overall score of aesthetic attributes for an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class VNImageAestheticsScoresObservation
```

## Topics

### Parsing Observation Content

var overallScore: Float

A score that incorporates the aesthetic score, failure score, and utility labels.

var isUtility: Bool

Returns a Boolean value that represents an image that may not have memorable or exciting content.

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

### Accessing the results

var results: [VNImageAestheticsScoresObservation]?

The results of the aesthetics request.

