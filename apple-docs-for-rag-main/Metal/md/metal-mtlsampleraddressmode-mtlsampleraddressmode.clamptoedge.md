

- Metal
- MTLSamplerAddressMode
-  MTLSamplerAddressMode.clampToEdge 

Case

# MTLSamplerAddressMode.clampToEdge

Texture coordinates are clamped between `0.0` and `1.0`, inclusive.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case clampToEdge
```

## See Also

### Address Mode Options

case mirrorClampToEdge

Between `-1.0` and `1.0`, the texture coordinates are mirrored across the axis; outside `-1.0` and `1.0`, texture coordinates are clamped.

case `repeat`

Texture coordinates wrap to the other side of the texture, effectively keeping only the fractional part of the texture coordinate.

case mirrorRepeat

Between `-1.0` and `1.0`, the texture coordinates are mirrored across the axis; outside `-1.0` and `1.0`, the image is repeated.

case clampToZero

Out-of-range texture coordinates return transparent zero `(0,0,0,0)` for images with an alpha channel and return opaque zero `(0,0,0,1)` for images without an alpha channel.

case clampToBorderColor

Out-of-range texture coordinates return the value specified by the borderColor property.

