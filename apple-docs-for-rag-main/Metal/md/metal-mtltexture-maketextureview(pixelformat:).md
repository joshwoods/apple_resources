

- Metal
- MTLTexture
-  makeTextureView(pixelFormat:) 

Instance Method

# makeTextureView(pixelFormat:)

Creates a new view of the texture, reinterpreting its data using a different pixel format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeTextureView(pixelFormat: MTLPixelFormat) -> (any MTLTexture)?
```

**Required**

## Parameters 

`pixelFormat`  

A new pixel format, which must be compatible with the original pixel format.

## Return Value

A new texture object that shares the same storage allocation of the texture.

## Discussion

When you create a texture normally, Metal allocates memory for the textureʼs pixel data. These storage allocations can be quite large. You can reduce memory use and avoid copying texture data by using a *texture view*—a texture object that shares another textureʼs storage allocation, reinterpreting the pixel data in some other format.

Not all pixel formats are compatible with one another. Reinterpretation of image data between pixel formats is supported within the following groups:

- All 8-, 16-, 32-, 64-, and 128-bit color formats are compatible with other formats with the same bit length.

- sRGB and non-sRGB forms of the same compressed format (for example, MTLPixelFormat.bc1_rgba and MTLPixelFormat.bc1_rgba_srgb)

- Combined depth-stencil texture formats and the related format used to access the stencil from a shader (for example, MTLPixelFormat.depth24Unorm_stencil8 and MTLPixelFormat.x24_stencil8)

This method doesn’t change the original texture image data in any way, but it may drastically change how the data is interpreted. For example, given a texture with the MTLPixelFormat.rg16Uint pixel format that contains image data for Red `0xFFFE` and Green `0x0001`, this method would reinterpret that data in an MTLPixelFormat.r32Uint format as Red `0x0001FFFE`.

Some format reinterpretations are supported but may not be useful. For example, this method considers the 32-bit packed color formats MTLPixelFormat.bgr10a2Unorm and MTLDataType.rg11b10Float to be compatible, but it’s unlikely that the same data can be interpreted by both formats in a meaningful way.

Some format reinterpretations require you to create the source texture with a special usage flag. Set that flag only when necessary, as it can affect performance. For more details, see pixelFormatView.

## See Also

### Related Documentation

var parentRelativeLevel: Int

The base level of the parent texture used to create this texture.

**Required**

var parent: (any MTLTexture)?

The parent texture used to create this texture, if any.

**Required**

var parentRelativeSlice: Int

The base slice of the parent texture used to create this texture.

**Required**

### Creating Textures by Reinterpreting Existing Texture Data

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type and pixel format.

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>, swizzle: MTLTextureSwizzleChannels) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type, pixel format, and swizzle pattern.

