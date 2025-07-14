

- Metal
- MTLPixelFormat
-  MTLPixelFormat.etc2_rgb8_srgb 

Case

# MTLPixelFormat.etc2_rgb8_srgb

Compressed format using ETC2 compression with three 8-bit components with conversion between sRGB and linear space.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 11.0+tvOSvisionOS 1.0+

``` source
case etc2_rgb8_srgb
```

## Discussion

Only MTLTextureType.type2D, MTLTextureType.type2DArray, and MTLTextureType.typeCube textures are supported.

## See Also

### Compressed EAC/ETC Pixel Formats

case eac_r11Unorm

Compressed format using EAC compression with one normalized unsigned integer component.

case eac_r11Snorm

Compressed format using EAC compression with one normalized signed integer component.

case eac_rg11Unorm

Compressed format using EAC compression with two normalized unsigned integer components.

case eac_rg11Snorm

Compressed format using EAC compression with two normalized signed integer components.

case eac_rgba8

Compressed format using EAC compression with four 8-bit components.

case eac_rgba8_srgb

Compressed format using EAC compression with four 8-bit components with conversion between sRGB and linear space.

case etc2_rgb8

Compressed format using ETC2 compression with three 8-bit components.

case etc2_rgb8a1

Compressed format using ETC2 compression with four 8-bit components.

case etc2_rgb8a1_srgb

Compressed format using ETC2 compression with four 8-bit components with conversion between sRGB and linear space.

