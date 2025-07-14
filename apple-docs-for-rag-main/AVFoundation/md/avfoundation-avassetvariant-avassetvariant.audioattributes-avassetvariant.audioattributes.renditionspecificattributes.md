

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
-  AVAssetVariant.AudioAttributes.RenditionSpecificAttributes 

Class

# AVAssetVariant.AudioAttributes.RenditionSpecificAttributes

An object that represents attributes specific to a particular rendition.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class RenditionSpecificAttributes
```

## Topics

### Accessing Attributes

var channelCount: Int?

The count of audio channels in the rendition.

var isBinaural: Bool

A Boolean value that indicates the variant is best suited for delivery to headphones.

var isImmersive: Bool

A Boolean value that indicates whether this variant contains virtualized or otherwise preprocessed audio content suitable for various purposes.

var isDownmix: Bool

A Boolean value that indicates whether the variant is a downmix derivative of other media of greater channel count.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Inspecting Audio Attributes

var formatIDs: [AudioFormatID]

The audio formats of the renditions present in the variant.

func renditionSpecificAttributes(for: AVMediaSelectionOption) -> AVAssetVariant.AudioAttributes.RenditionSpecificAttributes?

Returns specific attributes for the media option.

