

- AVFoundation
- AVAssetVariant
- AVAssetVariant.VideoAttributes
-  videoLayoutAttributes 

Instance Property

# videoLayoutAttributes

Attributes that describe the layout of the video content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var videoLayoutAttributes: [AVAssetVariant.VideoAttributes.LayoutAttributes] { get }
```

## Discussion

This property may contain more that one element if the variant contains a collection of differing video layout media attributes over time.

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

class LayoutAttributes

Attributes that describe the layout of video content.

