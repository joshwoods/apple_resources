

- AVFoundation
-  AVMediaType 

Structure

# AVMediaType

An identifier for various media types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMediaType
```

## Topics

### Media Types

static let audio: AVMediaType

The media contains audio media.

static let closedCaption: AVMediaType

The media contains closed-caption content.

static let depthData: AVMediaType

The media contains depth data.

static let haptic: AVMediaType

The media contains haptic content.

static let metadata: AVMediaType

The media contains metadata.

static let metadataObject: AVMediaType

The media contains metadata objects.

static let muxed: AVMediaType

The media contains muxed media.

static let subtitle: AVMediaType

The media contains subtitles.

static let text: AVMediaType

The media contains text.

static let timecode: AVMediaType

The media contains a time code.

static let video: AVMediaType

The media contains video.

### Initializers

init(String)

Creates a media type with a string.

init(rawValue: String)

Creates a media type with a raw string value.

### Type Properties

static let auxiliaryPicture: AVMediaType

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Media types

struct AVMediaCharacteristic

A structure that defines media data characteristics.

