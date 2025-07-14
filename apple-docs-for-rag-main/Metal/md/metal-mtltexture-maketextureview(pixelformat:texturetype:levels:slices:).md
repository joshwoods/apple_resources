

- Metal
- MTLTexture
-  makeTextureView(pixelFormat:textureType:levels:slices:) 

Instance Method

# makeTextureView(pixelFormat:textureType:levels:slices:)

Creates a new view of the texture, reinterpreting a subset of its data using a different type and pixel format.

iOS 9.0+iPadOS 9.0+Mac CatalystmacOS 10.11+tvOS 9.0+visionOS

``` source
func makeTextureView(
    pixelFormat: MTLPixelFormat,
    textureType: MTLTextureType,
    levels levelRange: Range,
    slices sliceRange: Range
) -> (any MTLTexture)?
```

## Parameters 

`pixelFormat`  

A new pixel format, which must be compatible with the original pixel format.

`textureType`  

A new texture type, which can be cast according to the original texture type as listed the table below.

`levelRange`  

A new base level range that restricts which mipmap levels are visible in the new texture.

`sliceRange`  

A new base slice range that restricts which array slices are visible in the new texture.

## Return Value

A new texture object that shares the same storage allocation of the calling texture object.

## Discussion

The texture type can be cast between the targets listed in the following table.

| Original texture type | New texture type |
|----|----|
| MTLTextureType.type1D | MTLTextureType.type1D |
| MTLTextureType.type2D | MTLTextureType.type2D or MTLTextureType.type2DArray |
| MTLTextureType.type2DArray, MTLTextureType.typeCube, or MTLTextureType.typeCubeArray | MTLTextureType.type2D, MTLTextureType.type2DArray, MTLTextureType.typeCube, or MTLTextureType.typeCubeArray |
| MTLTextureType.type3D | MTLTextureType.type3D |

The `length` value of the `sliceRange` parameter must be `6` if the new texture type value is MTLTextureType.typeCube, or a multiple of `6` if the new texture type value is MTLTextureType.typeCubeArray.

For more information on pixel format restrictions, see makeTextureView(pixelFormat:)

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

func makeTextureView(pixelFormat: MTLPixelFormat) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting its data using a different pixel format.

**Required**

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>, swizzle: MTLTextureSwizzleChannels) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type, pixel format, and swizzle pattern.

