

- AVFoundation
- AVAssetVariant
- AVAssetVariant.VideoAttributes
-  codecTypes 

Instance Property

# codecTypes

The video sample codec types present in the variant’s renditions.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@nonobjc
var codecTypes: [CMVideoCodecType] { get }
```

## See Also

### Inspecting the Attributes

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

