

- AVFoundation
- AVAssetVariant
-  AVAssetVariant.AudioAttributes 

Class

# AVAssetVariant.AudioAttributes

An object that defines the audio attributes for an asset variant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AudioAttributes
```

## Topics

### Inspecting Audio Attributes

var formatIDs: [AudioFormatID]

The audio formats of the renditions present in the variant.

func renditionSpecificAttributes(for: AVMediaSelectionOption) -> AVAssetVariant.AudioAttributes.RenditionSpecificAttributes?

Returns specific attributes for the media option.

class RenditionSpecificAttributes

An object that represents attributes specific to a particular rendition.

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

### Configuring Attributes

var audioAttributes: AVAssetVariant.AudioAttributes?

The audio rendition attributes for the variant.

var videoAttributes: AVAssetVariant.VideoAttributes?

The video rendition attributes for the variant.

class VideoAttributes

An object that defines the video attributes for an asset variant.

