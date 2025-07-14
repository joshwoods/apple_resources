

- AVFoundation
- AVAssetVariant
- AVAssetVariant.VideoAttributes
-  AVAssetVariant.VideoAttributes.LayoutAttributes 

Class

# AVAssetVariant.VideoAttributes.LayoutAttributes

Attributes that describe the layout of video content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class LayoutAttributes
```

## Topics

### Accessing attributes

var stereoViewComponents: CMStereoViewComponents

Attributes that describe the video’s stereo components.

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

