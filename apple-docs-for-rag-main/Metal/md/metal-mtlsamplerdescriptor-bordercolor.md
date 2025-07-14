

- Metal
- MTLSamplerDescriptor
-  borderColor 

Instance Property

# borderColor

The border color for clamped texture values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.12+tvOS 16.0+visionOS 1.0+

``` source
var borderColor: MTLSamplerBorderColor { get set }
```

## Discussion

This value is only used when the sampler address mode is MTLSamplerAddressMode.clampToBorderColor.

## See Also

### Declaring Addressing Modes

var rAddressMode: MTLSamplerAddressMode

The address mode for the texture depth (r) coordinate.

var sAddressMode: MTLSamplerAddressMode

The address mode for the texture width (s) coordinate.

var tAddressMode: MTLSamplerAddressMode

The address mode for the texture height (t) coordinate.

enum MTLSamplerAddressMode

Modes that determine the texture coordinate at each pixel when a fetch falls outside the bounds of a texture.

enum MTLSamplerBorderColor

Values that determine the border color for clamped texture values when the sampler address mode is MTLSamplerAddressMode.clampToBorderColor.

