

- Metal
- MTLIOCommandBuffer
-  load(\_:slice:level:size:sourceBytesPerRow:sourceBytesPerImage:destinationOrigin:sourceHandle:sourceHandleOffset:) 

Instance Method

# load(\_:slice:level:size:sourceBytesPerRow:sourceBytesPerImage:destinationOrigin:sourceHandle:sourceHandleOffset:)

Encodes a command that loads data from a file handle into a GPU texture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func load(
    _ texture: any MTLTexture,
    slice: Int,
    level: Int,
    size: MTLSize,
    sourceBytesPerRow: Int,
    sourceBytesPerImage: Int,
    destinationOrigin: MTLOrigin,
    sourceHandle: any MTLIOFileHandle,
    sourceHandleOffset: Int
)
```

**Required**

## Parameters 

`texture`  

A texture instance the method loads data into.

`slice`  

A slice within the texture.

`level`  

A level within the texture.

`size`  

The number of bytes the method loads from the file into the texture.

`sourceBytesPerRow`  

The number of bytes in a row of data from the source file.

`sourceBytesPerImage`  

The number of bytes in an image from the source file.

`destinationOrigin`  

A starting location within the texture the method copies data to.

`sourceHandle`  

A handle to a source file.

`sourceHandleOffset`  

A starting location relative to the beginning of the file, in bytes, the method copies data from.

## See Also

### Loading Assets

func load(any MTLBuffer, offset: Int, size: Int, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into a GPU buffer.

**Required**

func loadBytes(UnsafeMutableRawPointer, size: Int, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into CPU-accessible memory buffer.

**Required**

