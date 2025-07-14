

- Metal
- MTLTexture
-  getBytes(\_:bytesPerRow:from:mipmapLevel:) 

Instance Method

# getBytes(\_:bytesPerRow:from:mipmapLevel:)

Copies pixel data from the first slice of the texture to a buffer in system memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func getBytes(
    _ pixelBytes: UnsafeMutableRawPointer,
    bytesPerRow: Int,
    from region: MTLRegion,
    mipmapLevel level: Int
)
```

**Required**

## Parameters 

`pixelBytes`  

A pointer to a destination buffer in system memory.

`bytesPerRow`  

The number of bytes (*stride*) between two adjacent rows of pixel data in the destination buffer. For MTLTextureType.type1D and MTLTextureType.type1DArray, use `0`. For raw and packed pixel types, the stride is the number of pixels in one row. For compressed pixel formats, the stride is the number of bytes from the beginning of one row of blocks to the beginning of the next.

Your data type determines how you should compute `bytesPerRow`:

- For raw or packed pixel data, use a multiple of the pixel size less than max `* pixel size`.

- For compressed pixel data, use a multiple of the compression block size. When working with PowerVR Texture Compression (PVRTC), use `0.`

Nonzero values smaller than the texture width or any values not a multiple of the pixel or block size cause an error.

`region`  

The location of a block of pixels in the texture slice. For textures compressed as PVRTC, use the entire texture for the region.

`level`  

A zero-indexed value that selects the texture’s mipmap level as the method’s data source. Use `0` for textures that don’t have mipmaps.

## Discussion

Important

Don’t use this method for textures where storageMode is MTLStorageMode.private. Instead, copy data from the private texture with an MTLBlitCommandEncoder to another texture accessible from the CPU, and then call this method on the accessible texture.

This method runs on the CPU and immediately copies the pixel data from the texture to system memory but doesn’t synchronize with any GPU texture accesses. Ensure all operations that write or render to the texture complete before reading the texture’s contents, using one of the following methods:

- Synchronize on the GPU with a synchronize(resource:) or synchronize(texture:slice:level:) command in an MTLBlitCommandEncoder.

- Synchronize on the CPU with a callback passed to the addCompletedHandler(_:) method to handle completion asynchronously, or the waitUntilCompleted() method to block thread execution until the GPU work completes.

For multisample textures, the method consecutively positions each sample within a pixel in memory and treats the pixels as part of one row.

## See Also

### Copying Data from a Texture Image

func getBytes(UnsafeMutableRawPointer, bytesPerRow: Int, bytesPerImage: Int, from: MTLRegion, mipmapLevel: Int, slice: Int)

Copies pixel data from the texture to a buffer in system memory.

**Required**

