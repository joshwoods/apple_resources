

- Metal
- MTLTexture
-  replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) 

Instance Method

# replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:)

Copies pixel data into a section of a texture slice.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func replace(
    region: MTLRegion,
    mipmapLevel level: Int,
    slice: Int,
    withBytes pixelBytes: UnsafeRawPointer,
    bytesPerRow: Int,
    bytesPerImage: Int
)
```

**Required**

## Parameters 

`region`  

The location of a block of pixels in the texture slice. The region must be within the dimensions of the slice.

`level`  

A zero-indexed value that specifies which mipmap level is the destination. If the texture doesn’t have mipmaps, use `0`.

`slice`  

A zero-indexed value that specifies which texture slice is the destination:

- For a cube texture, `slice` is a value between `0` and `5`, inclusive, that defines which cube face is the destination.

- For a texture array, `slice` is the element index.

- For a cube texture array, slice defines both the cube face and an array index. To determine the correct slice for a cube texture array, treat it as having a stride of `6`: `slice = cubeFace + arrayIndex * 6.`

- For all other texture types, use `0`.

`pixelBytes`  

A pointer to the bytes in memory to copy.

`bytesPerRow`  

The stride, in bytes, of one row in the source data. For MTLTextureType.type1D and MTLTextureType.type1DArray, use `0`. For raw and packed pixel types, the stride is the number of pixels in one row. For compressed pixel formats, the stride is the number of bytes from the beginning of one row of blocks to the beginning of the next. When source data consists of only a single row, use `0`.

Your data type determines how you should compute `bytesPerRow`:

- For raw or packed pixel data, use a value greater than or equal to the size of data in one row, and less than `32767 * pixel size`.

- For compressed pixel data, use a multiple of the compression block size. When working with PowerVR Texture Compression (PVRTC), use `0.`

Nonzero values smaller than the texture width or not a multiple of the pixel size cause an error.

`bytesPerImage`  

The stride, in bytes, between images in the source data. Supply a nonzero value only when you copy data to an MTLTextureType.type3D type texture. Your data type determines how you should compute `bytesPerImage`:

- For data that consists only of a single image, use `0`.

- For ordinary or packed pixel formats, use a multiple of pixel size.

- For compressed pixel data, use a multiple of the compression block size. When working with PVRTC, use `0`.

When copying data to a type of texture other than MTLTextureType.type3D, use `0`.

## Mentioned in 

Optimizing Texture Data

Synchronizing a Managed Resource in macOS

## Discussion

This method runs on the CPU and immediately copies the pixel data into the texture. It doesn’t synchronize against any GPU accesses to the texture. Ensure all operations that write or render to the texture complete before reading the texture’s contents, using one of the following methods:

- Synchronize on the GPU with a synchronize(resource:) or synchronize(texture:slice:level:) command in an MTLBlitCommandEncoder.

- Synchronize on the CPU with a callback passed to the addCompletedHandler(_:) method to handle completion asynchronously, or the waitUntilCompleted() method to block thread execution until the GPU work completes.

If the texture image has a compressed pixel format, only write to block-aligned regions. If the size of a dimension of region isn’t a multiple of the block size, include both the edge block and additional space up to the texture dimensions in `bytesPerRow`.

To copy your data to a private texture, copy your data to a temporary texture with non-private storage, and then use an MTLBlitCommandEncoder to copy the data to the private texture for GPU use.

## See Also

### Related Documentation

Metal Shading Language Guide

enum MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

Metal Programming Guide

### Copying Data into a Texture Image

func replace(region: MTLRegion, mipmapLevel: Int, withBytes: UnsafeRawPointer, bytesPerRow: Int)

Copies a block of pixels into a section of texture slice 0.

**Required**

