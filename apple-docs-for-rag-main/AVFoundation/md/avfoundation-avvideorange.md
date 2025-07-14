

- AVFoundation
-  AVVideoRange 

Structure

# AVVideoRange

Constants that describe a video variant’s dynamic range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVVideoRange
```

## Topics

### Video Ranges

static let pq: AVVideoRange

Indicates Perceptual Quantizer (PQ) high-dynamic-range video.

static let hlg: AVVideoRange

Indicates Hybrid-Log Gamma (HLG) high-dynamic-range video.

static let sdr: AVVideoRange

Indicates standard-dynamic-range (SDR) video.

### Initializers

init(rawValue: String)

Creates a video range with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
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

var videoLayoutAttributes: [AVAssetVariant.VideoAttributes.LayoutAttributes]

Attributes that describe the layout of the video content.

class LayoutAttributes

Attributes that describe the layout of video content.

