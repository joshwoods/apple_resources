

- Metal
- MTLBlitCommandEncoder
-  copy(from:to:) 

Instance Method

# copy(from:to:)

Encodes a command that copies data from one texture to another.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func copy(
    from sourceTexture: any MTLTexture,
    to destinationTexture: any MTLTexture
)
```

**Required**

## Parameters 

`sourceTexture`  

A texture the command copies data from.

`destinationTexture`  

Another texture the command copies the data to that has the same pixel format and sample count as `sourceTexture`.

## Mentioned in 

Copying Data into or out of Mipmaps

## Discussion

The textures can be different sizes as long as the larger texture has a mipmap level that’s the same size as the smaller texture’s level `0` mipmap.

The command copies all identical mipmap sizes. If both textures are arrays, the command copies as many texture slices (array elements) as possible.

## See Also

### Copying Texture Data to Another Texture

func copy(from: any MTLTexture, sourceSlice: Int, sourceLevel: Int, to: any MTLTexture, destinationSlice: Int, destinationLevel: Int, sliceCount: Int, levelCount: Int)

Encodes a command that copies slices of a texture to another texture’s slices.

**Required**

func copy(from: any MTLTexture, sourceSlice: Int, sourceLevel: Int, sourceOrigin: MTLOrigin, sourceSize: MTLSize, to: any MTLTexture, destinationSlice: Int, destinationLevel: Int, destinationOrigin: MTLOrigin)

Encodes a command that copies image data from a texture’s slice into another slice.

**Required**

