

- AVFoundation
-  AVMetadataExtraAttributeKey 

Structure

# AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMetadataExtraAttributeKey
```

## Topics

### Extra Attribute Keys

static let valueURI: AVMetadataExtraAttributeKey

A key that identifies a resource to use as the item’s value.

static let baseURI: AVMetadataExtraAttributeKey

A key that identifies the base URI the item uses to resolve its related URIs.

static let info: AVMetadataExtraAttributeKey

A key that identifies more information about the item.

### Initializers

init(String)

Creates an extra attribute key with a string.

init(rawValue: String)

Creates an extra attribute key with a raw string value.

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

struct AVMetadataFormat

A structure that defines metadata formats.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

