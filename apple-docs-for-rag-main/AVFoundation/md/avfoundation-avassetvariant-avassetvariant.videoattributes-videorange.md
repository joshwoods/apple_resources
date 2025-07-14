

- AVFoundation
- AVAssetVariant
- AVAssetVariant.VideoAttributes
-  videoRange 

Instance Property

# videoRange

The video range of the variant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var videoRange: AVVideoRange { get }
```

## Discussion

The property defaults to sdr.

## See Also

### Inspecting the Attributes

var codecTypes: [CMVideoCodecType]

The video sample codec types present in the variant’s renditions.

var nominalFrameRate: Double?

The nominal frame rate of the variant’s renditions.

var presentationSize: CGSize

The presentation size of the variant’s renditions.

struct AVVideoRange

Constants that describe a video variant’s dynamic range.

var videoLayoutAttributes: [AVAssetVariant.VideoAttributes.LayoutAttributes]

Attributes that describe the layout of the video content.

class LayoutAttributes

Attributes that describe the layout of video content.

