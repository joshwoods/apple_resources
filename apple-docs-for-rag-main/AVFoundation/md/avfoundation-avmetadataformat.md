

- AVFoundation
-  AVMetadataFormat 

Structure

# AVMetadataFormat

A structure that defines metadata formats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMetadataFormat
```

## Mentioned in 

Retrieving media metadata

## Topics

### Metadata Formats

static let hlsMetadata: AVMetadataFormat

The HLS metadata format.

static let iTunesMetadata: AVMetadataFormat

The iTunes metadata format.

static let id3Metadata: AVMetadataFormat

The ID3 metadata format.

static let isoUserData: AVMetadataFormat

The ISO user data metadata format.

static let quickTimeMetadata: AVMetadataFormat

The QuickTime metadata format.

static let quickTimeUserData: AVMetadataFormat

The QuickTime user data metadata format.

static let unknown: AVMetadataFormat

An unknown metadata format.

### Initializers

init(rawValue: String)

Creates a metadata format with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Metadata

Retrieving media metadata

Load descriptive metadata for media assets and their tracks.

class AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

class AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

struct AVMetadataIdentifier

A structure that defines identifiers for metadata formats.

struct AVMetadataKey

A structure that defines a metadata key.

struct AVMetadataKeySpace

A structure that defines a metadata key space.

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

