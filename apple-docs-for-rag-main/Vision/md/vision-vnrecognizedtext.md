

- Vision
-  VNRecognizedText 

Class

# VNRecognizedText

Text recognized in an image through a text recognition request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNRecognizedText
```

## Overview

A single VNRecognizedTextObservation can contain multiple recognized text objects—one for each candidate.

## Topics

### Determining Recognized Text

var string: String

The top candidate for recognized text.

var confidence: VNConfidence

A normalized confidence score for the text recognition result.

### Locating Recognized Text

func boundingBox(for: Range&lt;String.Index>) throws -> VNRectangleObservation?

Calculates the bounding box around the characters in the range of a string.

## Relationships

### Inherits From

- NSObject

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

### Obtaining Recognized Text

func topCandidates(Int) -> [VNRecognizedText]

Requests the *n* top candidates for a recognized text string.

