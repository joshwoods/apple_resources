

- Metal
- MTLRenderCommandEncoder
-  setTileBuffers(\_:offsets:range:) 

Instance Method

# setTileBuffers(\_:offsets:range:)

Assigns multiple buffers to a range of entries in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS

``` source
func setTileBuffers(
    _ buffers: [(any MTLBuffer)?],
    offsets: [Int],
    range: Range
)
```

## Parameters 

`buffers`  

An array of MTLBuffer instances the command assigns to entries in the tile shader argument table for buffers.

`offsets`  

An array of integers. Each element represents the location, in bytes, from the start of the corresponding MTLBuffer element in `buffers` where the tile shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`range`  

A span of integers that represent the entries in the tile shader argument table for buffers. Each entry stores a record of the corresponding element in `buffers` and `offsets`.

## Discussion

By default, the buffer at each index is `nil`.

Note

The Objective-C version of this method is setTileBuffers:offsets:withRange:.

## See Also

### Assigning Buffers

func setTileBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the tile shader argument table.

**Required**

func setTileBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the tile shader argument table.

**Required**

func setTileBufferOffset(Int, index: Int)

Updates an entry in the tile shader argument table with a new location within the entry’s current buffer.

**Required**

