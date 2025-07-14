

- Metal
- MTLPixelFormat
-  MTLPixelFormat.pvrtc_rgb_2bpp Deprecated

Case

# MTLPixelFormat.pvrtc_rgb_2bpp

Compressed format using PVRTC compression and 2bpp for RGB components.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0Deprecated

``` source
case pvrtc_rgb_2bpp
```

Deprecated

Use one of the other formats with `astc`/`ASTC`, `etc2`/`ETC2`, or `bc`/`BC` instead.

## Discussion

Only MTLTextureType.type2D, MTLTextureType.type2DArray, and MTLTextureType.typeCube textures are supported. Subimages are not supported.

## See Also

### Compressed PVRTC Pixel Formats

case pvrtc_rgb_2bpp_srgb

Compressed format using PVRTC compression and 2bpp for RGB components with conversion between sRGB and linear space.

Deprecated

case pvrtc_rgb_4bpp

Compressed format using PVRTC compression and 4bpp for RGB components.

Deprecated

case pvrtc_rgb_4bpp_srgb

Compressed format using PVRTC compression and 4bpp for RGB components with conversion between sRGB and linear space.

Deprecated

case pvrtc_rgba_2bpp

Compressed format using PVRTC compression and 2bpp for RGBA components.

Deprecated

case pvrtc_rgba_2bpp_srgb

Compressed format using PVRTC compression and 2bpp for RGBA components with conversion between sRGB and linear space.

Deprecated

case pvrtc_rgba_4bpp

Compressed format using PVRTC compression and 4bpp for RGBA components.

Deprecated

case pvrtc_rgba_4bpp_srgb

Compressed format using PVRTC compression and 4bpp for RGBA components with conversion between sRGB and linear space.

Deprecated

