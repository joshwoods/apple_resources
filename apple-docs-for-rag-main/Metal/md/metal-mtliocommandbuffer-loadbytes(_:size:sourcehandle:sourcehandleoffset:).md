

- Metal
- MTLIOCommandBuffer
-  loadBytes(\_:size:sourceHandle:sourceHandleOffset:) 

Instance Method

# loadBytes(\_:size:sourceHandle:sourceHandleOffset:)

Encodes a command that loads data from a file handle into CPU-accessible memory buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func loadBytes(
    _ pointer: UnsafeMutableRawPointer,
    size: Int,
    sourceHandle: any MTLIOFileHandle,
    sourceHandleOffset: Int
)
```

**Required**

## Parameters 

`pointer`  

A pointer to memory the method loads data into.

`size`  

The number of bytes the method loads from the file.

`sourceHandle`  

A handle to a source file.

`sourceHandleOffset`  

A starting location relative to the beginning of the file, in bytes, the method copies data from.

## See Also

### Loading Assets

func load(any MTLBuffer, offset: Int, size: Int, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into a GPU buffer.

**Required**

func load(any MTLTexture, slice: Int, level: Int, size: MTLSize, sourceBytesPerRow: Int, sourceBytesPerImage: Int, destinationOrigin: MTLOrigin, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into a GPU texture.

**Required**

