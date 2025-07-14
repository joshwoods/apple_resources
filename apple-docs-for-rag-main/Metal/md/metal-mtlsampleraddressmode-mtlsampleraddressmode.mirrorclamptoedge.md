

- Metal
- MTLSamplerAddressMode
-  MTLSamplerAddressMode.mirrorClampToEdge 

Case

# MTLSamplerAddressMode.mirrorClampToEdge

Between `-1.0` and `1.0`, the texture coordinates are mirrored across the axis; outside `-1.0` and `1.0`, texture coordinates are clamped.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.11+tvOS 16.0+visionOS 1.0+

``` source
case mirrorClampToEdge
```

## See Also

### Address Mode Options

case clampToEdge

Texture coordinates are clamped between `0.0` and `1.0`, inclusive.

case `repeat`

Texture coordinates wrap to the other side of the texture, effectively keeping only the fractional part of the texture coordinate.

case mirrorRepeat

Between `-1.0` and `1.0`, the texture coordinates are mirrored across the axis; outside `-1.0` and `1.0`, the image is repeated.

case clampToZero

Out-of-range texture coordinates return transparent zero `(0,0,0,0)` for images with an alpha channel and return opaque zero `(0,0,0,1)` for images without an alpha channel.

case clampToBorderColor

Out-of-range texture coordinates return the value specified by the borderColor property.

