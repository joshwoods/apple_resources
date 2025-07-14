

- Metal
- MTLBlitCommandEncoder
-  copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:) 

Instance Method

# copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:)

Encodes a command that copies image data from a texture slice to a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func copy(
    from sourceTexture: any MTLTexture,
    sourceSlice: Int,
    sourceLevel: Int,
    sourceOrigin: MTLOrigin,
    sourceSize: MTLSize,
    to destinationBuffer: any MTLBuffer,
    destinationOffset: Int,
    destinationBytesPerRow: Int,
    destinationBytesPerImage: Int
)
```

**Required**

## Parameters 

`sourceTexture`  

A texture with an isFramebufferOnly property value of false that the command copies data from.

`sourceSlice`  

A slice within `sourceTexture`.

For textures that use a combined depth/stencil pixel format, call the copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:) method instead. Configure that method’s `options` parameter appropriately.

`sourceLevel`  

A mipmap level within `sourceTexture`.

`sourceOrigin`  

A location within `sourceTexture` that the command begins copying data from.

Assign `0` to each dimension that’s not relevant to `sourceTexture`. For example:

- If the source texture is a 2D texture, set the origin’s z property to `0`.

- If the source texture is a 1D texture, set the origin’s y and z properties to `0`.

`sourceSize`  

An MTLSize instance, which can represent a 3D region, that instructs the command how many pixels to copy from `sourceTexture`, starting at `sourceOrigin`.

Assign `1` to each dimension that’s not relevant to `sourceTexture`. For example:

- If the source texture is a 2D texture, set the size’s depth property to `1`.

- If the source texture is a 1D texture, set the size’s height and depth properties to `1`.

If `sourceTexture` uses a compressed pixel format, set `sourceSize` to a multiple of the pixel format’s block size. If the block extends outside the bounds of the texture, clamp `sourceSize` to the edge of the texture.

`destinationBuffer`  

A buffer the command copies data to.

`destinationOffset`  

A byte offset within `destinationBuffer` the command copies to, which needs to be a multiple of the source texture’s pixel size, in bytes.

`destinationBytesPerRow`  

The number of bytes between adjacent rows of pixels in the destination buffer’s memory, which needs to be:

- A multiple of the source texture’s pixel size, in bytes

- Less than or equal to the product of the source texture’s pixel size, in bytes, and the largest pixel width the source texture’s type allows

If `sourceTexture` uses a compressed pixel format, set `destinationBytesPerRow` to the number of bytes between the starts of two row blocks.

`destinationBytesPerImage`  

The number of bytes between each 2D image of a 3D texture. This value needs to be a multiple of the source texture’s pixel size, in bytes.

Set this value to `0` for 2D textures, which means `sourceSize.`depth is equal to `1`.

## Mentioned in 

Copying Data to a Private Resource

## Discussion

This method is the equivalent of passing an empty OptionSet to the `options` parameter of copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:). In Swift, pass `[]` to represent an empty option set, and in Objective-C, pass MTLBlitOptionNone.

Important

If the pixel format of `sourceTexture` is a PVRTC format, use copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:) instead.

## See Also

### Copying Texture Data to a Buffer

func copy(from: any MTLTexture, sourceSlice: Int, sourceLevel: Int, sourceOrigin: MTLOrigin, sourceSize: MTLSize, to: any MTLBuffer, destinationOffset: Int, destinationBytesPerRow: Int, destinationBytesPerImage: Int, options: MTLBlitOption)

Encodes a command that copies image data from a texture slice to a buffer, and provides options for special texture formats.

**Required**

