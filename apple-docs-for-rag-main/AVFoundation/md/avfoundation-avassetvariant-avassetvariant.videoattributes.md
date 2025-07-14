

- AVFoundation
- AVAssetVariant
-  AVAssetVariant.VideoAttributes 

Class

# AVAssetVariant.VideoAttributes

An object that defines the video attributes for an asset variant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class VideoAttributes
```

## Topics

### Inspecting the Attributes

var codecTypes: [CMVideoCodecType]

The video sample codec types present in the variant’s renditions.

var nominalFrameRate: Double?

The nominal frame rate of the variant’s renditions.

var presentationSize: CGSize

The presentation size of the variant’s renditions.

var videoRange: AVVideoRange

The video range of the variant.

struct AVVideoRange

Constants that describe a video variant’s dynamic range.

var videoLayoutAttributes: [AVAssetVariant.VideoAttributes.LayoutAttributes]

Attributes that describe the layout of the video content.

class LayoutAttributes

Attributes that describe the layout of video content.

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

class AudioAttributes

An object that defines the audio attributes for an asset variant.

var videoAttributes: AVAssetVariant.VideoAttributes?

The video rendition attributes for the variant.

