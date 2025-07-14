

- Metal
- MTLTexture
-  makeTextureView(pixelFormat:textureType:levels:slices:swizzle:) 

Instance Method

# makeTextureView(pixelFormat:textureType:levels:slices:swizzle:)

Creates a new view of the texture, reinterpreting a subset of its data using a different type, pixel format, and swizzle pattern.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS

``` source
func makeTextureView(
    pixelFormat: MTLPixelFormat,
    textureType: MTLTextureType,
    levels levelRange: Range,
    slices sliceRange: Range,
    swizzle: MTLTextureSwizzleChannels
) -> (any MTLTexture)?
```

## Parameters 

`pixelFormat`  

A new pixel format, which must be compatible with the original pixel format.

`textureType`  

A new texture type.

`levelRange`  

A new base level range that restricts which mipmap levels are visible in the new texture.

`sliceRange`  

A new base slice range that restricts which array slices are visible in the new texture.

`swizzle`  

The swizzle pattern the GPU uses to reorder the data when sampling or reading the texture.

## Discussion

For more information on texture views, see makeTextureView(pixelFormat:textureType:levels:slices:)

The swizzle pattern of the view is combined with that of the parent texture to generate the final swizzle pattern. For example: An `[R,G,A,B]` swizzle of a texture with a `[R,1,1,G]` swizzle pattern is `[R,1,G,1]`.

## See Also

### Creating Textures by Reinterpreting Existing Texture Data

func makeTextureView(pixelFormat: MTLPixelFormat) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting its data using a different pixel format.

**Required**

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type and pixel format.

