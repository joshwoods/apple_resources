

- Metal
-  MTLSamplerBorderColor 

Enumeration

# MTLSamplerBorderColor

Values that determine the border color for clamped texture values when the sampler address mode is MTLSamplerAddressMode.clampToBorderColor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.12+tvOS 16.0+visionOS 1.0+

``` source
enum MTLSamplerBorderColor
```

## Topics

### Specifying Border Color Options

case transparentBlack

A transparent black color `(0,0,0,0)` for texture values outside the border.

case opaqueBlack

An opaque black color `(0,0,0,1)` for texture values outside the border

case opaqueWhite

An opaque white color `(1,1,1,1)` for texture values outside the border.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Declaring Addressing Modes

var rAddressMode: MTLSamplerAddressMode

The address mode for the texture depth (r) coordinate.

var sAddressMode: MTLSamplerAddressMode

The address mode for the texture width (s) coordinate.

var tAddressMode: MTLSamplerAddressMode

The address mode for the texture height (t) coordinate.

var borderColor: MTLSamplerBorderColor

The border color for clamped texture values.

enum MTLSamplerAddressMode

Modes that determine the texture coordinate at each pixel when a fetch falls outside the bounds of a texture.

