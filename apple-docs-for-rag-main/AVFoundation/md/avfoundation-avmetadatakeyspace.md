

- AVFoundation
-  AVMetadataKeySpace 

Structure

# AVMetadataKeySpace

A structure that defines a metadata key space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMetadataKeySpace
```

## Topics

### Common Key Space

static let common: AVMetadataKeySpace

The common key space.

### Format-Specific Key Spaces

static let audioFile: AVMetadataKeySpace

The AudioToolbox audio file key space.

static let hlsDateRange: AVMetadataKeySpace

The HTTP Live Streaming key space.

static let iTunes: AVMetadataKeySpace

The iTunes key space.

static let icy: AVMetadataKeySpace

The Icecast/ShoutCAST streaming key space.

static let id3: AVMetadataKeySpace

The ID3 key space.

static let isoUserData: AVMetadataKeySpace

The ISO key space.

static let quickTimeMetadata: AVMetadataKeySpace

The QuickTime metadata key space.

static let quickTimeUserData: AVMetadataKeySpace

The QuickTime user data key space.

### Initializers

init(String)

Creates a key space with a string.

init(rawValue: String)

Creates a key space with a raw string value.

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

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

struct AVMetadataFormat

A structure that defines metadata formats.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

