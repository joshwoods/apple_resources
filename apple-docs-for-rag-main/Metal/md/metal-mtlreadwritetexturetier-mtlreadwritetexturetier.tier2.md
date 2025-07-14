

- Metal
- MTLReadWriteTextureTier
-  MTLReadWriteTextureTier.tier2 

Case

# MTLReadWriteTextureTier.tier2

Tier 2 read/write textures are supported.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
case tier2
```

## Discussion

Read/write texture tier 2 supports the following pixel formats in addition to those supported by MTLReadWriteTextureTier.tier1:

- MTLPixelFormat.rgba32Float

- MTLPixelFormat.rgba32Uint

- MTLPixelFormat.rgba32Sint

- MTLPixelFormat.rgba16Float

- MTLPixelFormat.rgba16Uint

- MTLPixelFormat.rgba16Sint

- MTLPixelFormat.rgba8Unorm

- MTLPixelFormat.rgba8Uint

- MTLPixelFormat.rgba8Sint

- MTLPixelFormat.r16Float

- MTLPixelFormat.r16Uint

- MTLPixelFormat.r16Sint

- MTLPixelFormat.r8Unorm

- MTLPixelFormat.r8Uint

- MTLPixelFormat.r8Sint

## See Also

### Enumeration Cases

case tier1

Tier 1 read/write textures are supported.

case tierNone

Read-write textures are not supported.

