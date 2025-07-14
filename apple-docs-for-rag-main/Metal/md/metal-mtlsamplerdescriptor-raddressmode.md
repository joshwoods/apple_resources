

- Metal
- MTLSamplerDescriptor
-  rAddressMode 

Instance Property

# rAddressMode

The address mode for the texture depth (r) coordinate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var rAddressMode: MTLSamplerAddressMode { get set }
```

## Discussion

The default value is MTLSamplerAddressMode.clampToEdge.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Declaring Addressing Modes

var sAddressMode: MTLSamplerAddressMode

The address mode for the texture width (s) coordinate.

var tAddressMode: MTLSamplerAddressMode

The address mode for the texture height (t) coordinate.

var borderColor: MTLSamplerBorderColor

The border color for clamped texture values.

enum MTLSamplerAddressMode

Modes that determine the texture coordinate at each pixel when a fetch falls outside the bounds of a texture.

enum MTLSamplerBorderColor

Values that determine the border color for clamped texture values when the sampler address mode is MTLSamplerAddressMode.clampToBorderColor.

