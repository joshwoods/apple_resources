

- AVFoundation
-  AVVideoCodecType 

Structure

# AVVideoCodecType

A set of constants that describe the codecs the system supports for video capture.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVVideoCodecType
```

## Mentioned in 

Recording movies in alternative formats

## Topics

### Video codecs

static let h264: AVVideoCodecType

The H.264 video codec.

static let hevc: AVVideoCodecType

The HEVC video codec.

static let hevcWithAlpha: AVVideoCodecType

The HEVC video codec that supports an alpha channel.

static let jpeg: AVVideoCodecType

The JPEG video codec.

static let proRes422: AVVideoCodecType

The Apple ProRes 422 video codec.

static let proRes422LT: AVVideoCodecType

The Apple ProRes 422 LT video codec.

static let proRes422HQ: AVVideoCodecType

The Apple ProRes 422 HQ video codec.

static let proRes422Proxy: AVVideoCodecType

The Apple ProRes 422 Proxy video codec.

static let proRes4444: AVVideoCodecType

The Apple ProRes 4444 video codec.

static let appleProRes4444XQ: AVVideoCodecType

The Apple ProRes 4444 XQ video codec.

### Deprecated

let AVVideoCodecH264: String

A key to access the name of the H.264 codec for compressing video.

Deprecated

let AVVideoCodecHEVC: String

A key to access the name of the HEVC codec used to encode the video.

Deprecated

let AVVideoCodecJPEG: String

A key to access the name of the JPEG codec for compressing video.

Deprecated

let AVVideoCodecAppleProRes422: String

A key to access the name of the Apple ProRes422 codec used to encode the video.

Deprecated

let AVVideoCodecAppleProRes4444: String

A key to access the name of the Apple ProRes4444 codec used to encode the video.

Deprecated

### Initializers

init(rawValue: String)

Creates a codec type from its raw string value.

### Type Properties

static let JPEGXL: AVVideoCodecType

The JPEG XL video codec.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Video codecs

let AVVideoCodecKey: String

A key to access the name of the codec for compressing video.

