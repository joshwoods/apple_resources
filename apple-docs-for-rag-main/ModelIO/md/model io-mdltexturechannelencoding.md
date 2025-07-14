

- Model I/O
-  MDLTextureChannelEncoding 

Enumeration

# MDLTextureChannelEncoding

Options for the data size and type of texel channel values, used by the channelEncoding property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLTextureChannelEncoding
```

## Topics

### Constants

case uInt8

Each channel value per texel is an 8-bit unsigned integer.

case uInt16

Each channel value per texel is a 16-bit unsigned integer.

case uInt24

Each channel value per texel is a 24-bit unsigned integer.

case uInt32

Each channel value per texel is a 32-bit unsigned integer.

case float16

Each channel value per texel is a 16-bit floating-point value.

case float32

Each channel value per texel is a 32-bit floating-point value.

### Enumeration Cases

case float16SR

### Initializers

init?(rawValue: Int)

### Type Properties

static var uint16: MDLTextureChannelEncoding

Each channel value per texel is a 16-bit unsigned integer.

static var uint24: MDLTextureChannelEncoding

Each channel value per texel is a 24-bit unsigned integer.

static var uint32: MDLTextureChannelEncoding

Each channel value per texel is a 32-bit unsigned integer.

static var uint8: MDLTextureChannelEncoding

Each channel value per texel is an 8-bit unsigned integer.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

