

- Metal
-  MTLPixelFormat 

Enumeration

# MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLPixelFormat
```

## Overview

There are three varieties of pixel formats: ordinary, packed, and compressed. For ordinary and packed formats, the name of the pixel format specifies the order of components (such as `R`, `RG`, `RGB`, `RGBA`, `BGRA`), bits per component (such as `8`, `16`, `32`), and data type for the component (such as `Float`, `Sint`, `Snorm`, `Uint`, `Unorm`). If the pixel format name has the `_sRGB` suffix, then reading and writing pixel data applies sRGB gamma compression and decompression. The alpha component of sRGB pixel formats is always treated as a linear value. For compressed formats, the name of the pixel format specifies a compression family (such as `ASTC`, `BC`, `EAC`, `ETC2`, `PVRTC`).

Note

Pixel format availability and capabilities vary by feature set. See Pixel Format Capabilities for more information.

### Storage Characteristics

The number and size of each pixel component determines the storage size of each pixel format. For example, the storage size of MTLPixelFormat.bgra8Unorm is 32 bits (four 8-bit components) and the storage size of MTLPixelFormat.bgr5A1Unorm is 16 bits (three 5-bit components and one 1-bit component).

For normalized signed integer formats (`Snorm`), values in the range `[-1.0, 1.0]` map to `[MIN_INT, MAX_INT]`, where `MIN_INT` is the greatest negative integer and `MAX_INT` is the greatest positive integer for the number of bits in the storage size. Positive values and zero distribute uniformly in the range `[0.0, 1.0]`, and negative integer values greater than `(MIN_INT + 1)` distribute uniformly in the range `(-1.0, 0.0)`.

Important

For `Snorm` formats, the values `MIN_INT` and `(MIN_INT + 1)` both map to `-1.0`.

For normalized unsigned integer formats (`Unorm`), values in the range `[0.0, 1.0]` are uniformly mapped to `[0, MAX_UINT]`, where `MAX_UINT` is the greatest unsigned integer for the number of bits in the storage size.

Format data is little-endian (the least-significant byte in the least-significant address). For formats with components that are themselves byte-aligned and more than one byte, the components are also little-endian.

See Table 7.7 in the Metal Shading Language Specification (PDF) for details on pixel format normalization.

## Topics

### Ordinary 8-Bit Pixel Formats

case a8Unorm

Ordinary format with one 8-bit normalized unsigned integer component.

case r8Unorm

Ordinary format with one 8-bit normalized unsigned integer component.

case r8Unorm_srgb

Ordinary format with one 8-bit normalized unsigned integer component with conversion between sRGB and linear space.

case r8Snorm

Ordinary format with one 8-bit normalized signed integer component.

case r8Uint

Ordinary format with one 8-bit unsigned integer component.

case r8Sint

Ordinary format with one 8-bit signed integer component.

### Ordinary 16-Bit Pixel Formats

case r16Unorm

Ordinary format with one 16-bit normalized unsigned integer component.

case r16Snorm

Ordinary format with one 16-bit normalized signed integer component.

case r16Uint

Ordinary format with one 16-bit unsigned integer component.

case r16Sint

Ordinary format with one 16-bit signed integer component.

case r16Float

Ordinary format with one 16-bit floating-point component.

case rg8Unorm

Ordinary format with two 8-bit normalized unsigned integer components.

case rg8Unorm_srgb

Ordinary format with two 8-bit normalized unsigned integer components with conversion between sRGB and linear space.

case rg8Snorm

Ordinary format with two 8-bit normalized signed integer components.

case rg8Uint

Ordinary format with two 8-bit unsigned integer components.

case rg8Sint

Ordinary format with two 8-bit signed integer components.

### Packed 16-Bit Pixel Formats

case b5g6r5Unorm

Packed 16-bit format with normalized unsigned integer color components: 5 bits for blue, 6 bits for green, 5 bits for red, packed into 16 bits.

case a1bgr5Unorm

Packed 16-bit format with normalized unsigned integer color components: 5 bits each for BGR and 1 for alpha, packed into 16 bits.

case abgr4Unorm

Packed 16-bit format with normalized unsigned integer color components: 4 bits each for ABGR, packed into 16 bits.

case bgr5A1Unorm

Packed 16-bit format with normalized unsigned integer color components: 5 bits each for BGR and 1 for alpha, packed into 16 bits.

### Ordinary 32-Bit Pixel Formats

case r32Uint

Ordinary format with one 32-bit unsigned integer component.

case r32Sint

Ordinary format with one 32-bit signed integer component.

case r32Float

Ordinary format with one 32-bit floating-point component.

case rg16Unorm

Ordinary format with two 16-bit normalized unsigned integer components.

case rg16Snorm

Ordinary format with two 16-bit normalized signed integer components.

case rg16Uint

Ordinary format with two 16-bit unsigned integer components.

case rg16Sint

Ordinary format with two 16-bit signed integer components.

case rg16Float

Ordinary format with two 16-bit floating-point components.

case rgba8Unorm

Ordinary format with four 8-bit normalized unsigned integer components in RGBA order.

case rgba8Unorm_srgb

Ordinary format with four 8-bit normalized unsigned integer components in RGBA order with conversion between sRGB and linear space.

case rgba8Snorm

Ordinary format with four 8-bit normalized signed integer components in RGBA order.

case rgba8Uint

Ordinary format with four 8-bit unsigned integer components in RGBA order.

case rgba8Sint

Ordinary format with four 8-bit signed integer components in RGBA order.

case bgra8Unorm

Ordinary format with four 8-bit normalized unsigned integer components in BGRA order.

case bgra8Unorm_srgb

Ordinary format with four 8-bit normalized unsigned integer components in BGRA order with conversion between sRGB and linear space.

### Packed 32-Bit Pixel Formats

case bgr10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit blue, 10-bit green, 10-bit red, and 2-bit alpha.

case rgb10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rgb10a2Uint

A 32-bit packed pixel format with four unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rg11b10Float

32-bit format with floating-point color components, 11 bits each for red and green and 10 bits for blue.

case rgb9e5Float

Packed 32-bit format with floating-point color components: 9 bits each for RGB and 5 bits for an exponent shared by RGB, packed into 32 bits.

### Ordinary 64-Bit Pixel Formats

case rg32Uint

Ordinary format with two 32-bit unsigned integer components.

case rg32Sint

Ordinary format with two 32-bit signed integer components.

case rg32Float

Ordinary format with two 32-bit floating-point components.

case rgba16Unorm

Ordinary format with four 16-bit normalized unsigned integer components in RGBA order.

case rgba16Snorm

Ordinary format with four 16-bit normalized signed integer components in RGBA order.

case rgba16Uint

Ordinary format with four 16-bit unsigned integer components in RGBA order.

case rgba16Sint

Ordinary format with four 16-bit signed integer components in RGBA order.

case rgba16Float

Ordinary format with four 16-bit floating-point components in RGBA order.

### Ordinary 128-Bit Pixel Formats

case rgba32Uint

Ordinary format with four 32-bit unsigned integer components in RGBA order.

case rgba32Sint

Ordinary format with four 32-bit signed integer components in RGBA order.

case rgba32Float

Ordinary format with four 32-bit floating-point components in RGBA order.

### Compressed PVRTC Pixel Formats

case pvrtc_rgb_2bpp

Compressed format using PVRTC compression and 2bpp for RGB components.

Deprecated

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

case etc2_rgb8_srgb

Compressed format using ETC2 compression with three 8-bit components with conversion between sRGB and linear space.

case etc2_rgb8a1

Compressed format using ETC2 compression with four 8-bit components.

case etc2_rgb8a1_srgb

Compressed format using ETC2 compression with four 8-bit components with conversion between sRGB and linear space.

### Compressed ASTC Pixel Formats

ASTC formats use a fixed number of bytes per block, so image quality decreases as the block dimensions grow.

case astc_4x4_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 4, and a block height of 4.

case astc_5x4_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 5, and a block height of 4.

case astc_5x5_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 5, and a block height of 5.

case astc_6x5_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 6, and a block height of 5.

case astc_6x6_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 6, and a block height of 6.

case astc_8x5_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 8, and a block height of 5.

case astc_8x6_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 8, and a block height of 6.

case astc_8x8_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 8, and a block height of 8.

case astc_10x5_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 10, and a block height of 5.

case astc_10x6_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 10, and a block height of 6.

case astc_10x8_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 10, and a block height of 8.

case astc_10x10_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 10, and a block height of 10.

case astc_12x10_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 12, and a block height of 10.

case astc_12x12_srgb

ASTC-compressed format with low-dynamic-range content, conversion between sRGB and linear space, a block width of 12, and a block height of 12.

case astc_4x4_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 4, and a block height of 4.

case astc_5x4_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 5, and a block height of 4.

case astc_5x5_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 5, and a block height of 5.

case astc_6x5_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 6, and a block height of 5.

case astc_6x6_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 6, and a block height of 6.

case astc_8x5_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 8, and a block height of 5.

case astc_8x6_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 8, and a block height of 6.

case astc_8x8_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 8, and a block height of 8.

case astc_10x5_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 10, and a block height of 5.

case astc_10x6_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 10, and a block height of 6.

case astc_10x8_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 10, and a block height of 8.

case astc_10x10_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 10, and a block height of 10.

case astc_12x10_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 12, and a block height of 10.

case astc_12x12_ldr

ASTC-compressed format with low-dynamic-range content, a block width of 12, and a block height of 12.

case astc_4x4_hdr

ASTC-compressed format with high-dynamic-range content, a block width of 4, and a block height of 4.

case astc_5x4_hdr

ASTC-compressed format with high-dynamic range content, a block width of 5, and a block height of 4.

case astc_5x5_hdr

ASTC-compressed format with high-dynamic range content, a block width of 5, and a block height of 6.

case astc_6x5_hdr

ASTC-compressed format with high-dynamic range content, a block width of 6, and a block height of 5.

case astc_6x6_hdr

ASTC-compressed format with high-dynamic range content, a block width of 6, and a block height of 6.

case astc_8x5_hdr

ASTC-compressed format with high-dynamic range content, a block width of 8, and a block height of 5.

case astc_8x6_hdr

ASTC-compressed format with high-dynamic range content, a block width of 8, and a block height of 6.

case astc_8x8_hdr

ASTC-compressed format with high-dynamic range content, a block width of 8, and a block height of 8.

case astc_10x5_hdr

ASTC-compressed format with high-dynamic range content, a block width of 10, and a block height of 5.

case astc_10x6_hdr

ASTC-compressed format with high-dynamic range content, a block width of 10, and a block height of 6.

case astc_10x8_hdr

ASTC-compressed format with high-dynamic range content, a block width of 10, and a block height of 8.

case astc_10x10_hdr

ASTC-compressed format with high-dynamic range content, a block width of 10, and a block height of 10.

case astc_12x10_hdr

ASTC-compressed format with high-dynamic range content, a block width of 12, and a block height of 10.

case astc_12x12_hdr

ASTC-compressed format with high-dynamic range content, a block width of 12, and a block height of 12.

### Compressed BC Pixel Formats

case bc1_rgba

Compressed format with two 16-bit color components and one 32-bit descriptor component.

case bc1_rgba_srgb

Compressed format with two 16-bit color components and one 32-bit descriptor component, with conversion between sRGB and linear space.

case bc2_rgba

Compressed format with two 64-bit chunks. The first chunk contains two 8-bit alpha components and one 48-bit descriptor component. The second chunk contains two 16-bit color components and one 32-bit descriptor component.

case bc2_rgba_srgb

Compressed format with two 64-bit chunks, with conversion between sRGB and linear space. The first chunk contains two 8-bit alpha components and one 48-bit descriptor component. The second chunk contains two 16-bit color components and one 32-bit descriptor component.

case bc3_rgba

Compressed format with two 64-bit chunks. The first chunk contains two 8-bit alpha components and one 48-bit descriptor component. The second chunk contains two 16-bit color components and one 32-bit descriptor component.

case bc3_rgba_srgb

Compressed format with two 64-bit chunks, with conversion between sRGB and linear space. The first chunk contains two 8-bit alpha components and one 48-bit descriptor component. The second chunk contains two 16-bit color components and one 32-bit descriptor component.

case bc4_rUnorm

Compressed format with one normalized unsigned integer component.

case bc4_rSnorm

Compressed format with one normalized signed integer component.

case bc5_rgUnorm

Compressed format with two normalized unsigned integer components.

case bc5_rgSnorm

Compressed format with two normalized signed integer components.

case bc6H_rgbFloat

Compressed format with four floating-point components.

case bc6H_rgbuFloat

Compressed format with four unsigned floating-point components.

case bc7_rgbaUnorm

Compressed format with four normalized unsigned integer components.

case bc7_rgbaUnorm_srgb

Compressed format with four normalized unsigned integer components, with conversion between sRGB and linear space.

### YUV Pixel Formats

case gbgr422

A pixel format where the red and green components are subsampled horizontally.

case bgrg422

A pixel format where the red and green components are subsampled horizontally.

### Depth and Stencil Pixel Formats

case depth16Unorm

A pixel format for a depth-render target that has a 16-bit normalized, unsigned-integer component.

case depth32Float

A pixel format with one 32-bit floating-point component, used for a depth render target.

case stencil8

A pixel format with an 8-bit unsigned integer component, used for a stencil render target.

case depth24Unorm_stencil8

A 32-bit combined depth and stencil pixel format with a 24-bit normalized unsigned integer for depth and an 8-bit unsigned integer for stencil.

case depth32Float_stencil8

A 40-bit combined depth and stencil pixel format with a 32-bit floating-point value for depth and an 8-bit unsigned integer for stencil.

case x32_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 32-bit depth and 8-bit stencil value.

case x24_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 24-bit depth and 8-bit stencil value.

### Extended Range and Wide Color Pixel Formats

case bgra10_xr

A 64-bit extended-range pixel format with four fixed-point components of 10-bit blue, 10-bit green, 10-bit red, and 10-bit alpha.

case bgra10_xr_srgb

A 64-bit extended-range pixel format with sRGB conversion and four fixed-point components of 10-bit blue, 10-bit green, 10-bit red, and 10-bit alpha.

case bgr10_xr

A 32-bit extended-range pixel format with three fixed-point components of 10-bit blue, 10-bit green, and 10-bit red.

case bgr10_xr_srgb

A 32-bit extended-range pixel format with sRGB conversion and three fixed-point components of 10-bit blue, 10-bit green, and 10-bit red.

### Invalid Pixel Format

case invalid

The default value of the pixel format for the `MTLRenderPipelineState`. You cannot create a texture with this value.

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

### Texture Basics

Understanding Color-Renderable Pixel Format Sizes

Know the size limits of color render targets in Apple GPUs based on the target’s pixel format.

Optimizing Texture Data

Optimize a texture’s data to improve GPU or CPU access.

protocol MTLTexture

A resource that holds formatted image data.

enum MTLTextureCompressionType

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

class MTKTextureLoader

An object that creates textures from existing data in common image formats.

class MTLSharedTextureHandle

A texture handle that can be shared across process address space boundaries.

