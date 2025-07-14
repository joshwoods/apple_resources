

- Core Media
- CMFormatDescription
-  CMFormatDescription.Extensions 

Structure

# CMFormatDescription.Extensions

A type that describes format description extensions.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Extensions
```

## Topics

### Comparing Extensions

static func == (CMFormatDescription, CMFormatDescription) -> Bool

Equality is derived from

### Creating Extensions

init()

init(base: [CFString : CFPropertyList]?)

### Finding Extension Elements

subscript(CFString) -> CFPropertyList?

subscript(CMFormatDescription.Extensions.Key) -> CMFormatDescription.Extensions.Value?

### Constants

struct Key

struct Value

## Relationships

### Conforms To

- Collection
- Copyable
- Equatable
- Hashable
- Sendable
- Sequence

## See Also

### Constants

static var extensionKeysCommonWithImageBuffers: [CMFormatDescription.Extensions.Key]

A constant that represents keys you use with video format description extensions and image buffers.

static var typeID: CFTypeID

A type identifier that corresponds to a description object.

struct MediaType

A type that describes format description media.

struct MediaSubType

A type that describes format description media subtypes.

struct TimeCode

A type that describes format description time codes.

struct EqualityMask

A type that describes format description equality masks.

struct ParameterSetCollection

A type that describes format description parameter sets.

