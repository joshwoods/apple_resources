

- Core Media
- CMFormatDescription
-  CMFormatDescription.MediaType 

Structure

# CMFormatDescription.MediaType

A type that describes format description media.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MediaType
```

## Topics

### Media Types

static let audio: CMFormatDescription.MediaType

static let closedCaption: CMFormatDescription.MediaType

static let metadata: CMFormatDescription.MediaType

static let muxed: CMFormatDescription.MediaType

static let subtitle: CMFormatDescription.MediaType

static let text: CMFormatDescription.MediaType

static let timeCode: CMFormatDescription.MediaType

static let video: CMFormatDescription.MediaType

static let taggedBufferGroup: CMFormatDescription.MediaType

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

static var extensionKeysCommonWithImageBuffers: [CMFormatDescription.Extensions.Key]

A constant that represents keys you use with video format description extensions and image buffers.

static var typeID: CFTypeID

A type identifier that corresponds to a description object.

struct MediaSubType

A type that describes format description media subtypes.

struct TimeCode

A type that describes format description time codes.

struct EqualityMask

A type that describes format description equality masks.

struct Extensions

A type that describes format description extensions.

struct ParameterSetCollection

A type that describes format description parameter sets.

