

- AVFoundation
-  AVCompositionTrackFormatDescriptionReplacement 

Class

# AVCompositionTrackFormatDescriptionReplacement

An object that represents a format description and its replacement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class AVCompositionTrackFormatDescriptionReplacement
```

## Topics

### Managing Format Descriptions

var originalFormatDescription: CMFormatDescription

The format description to replace.

var replacementFormatDescription: CMFormatDescription

The replacement format description.

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
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Managing Format Descriptions

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

var formatDescriptionReplacements: [AVCompositionTrackFormatDescriptionReplacement]

The replacement format descriptions.

