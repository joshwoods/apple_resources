

- Metal
- MTLRenderCommandEncoder
-  setTileBuffer(\_:offset:index:) 

Instance Method

# setTileBuffer(\_:offset:index:)

Assigns a buffer to an entry in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setTileBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

An MTLBuffer instance the command assigns to an entry in the tile shader argument table for buffers.

`offset`  

An integer that represents the location, in bytes, from the start of `buffer` where the tile shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`index`  

An integer that represents the entry in the tile shader argument table for buffers that stores a record of `buffer` and `offset`.

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Discussion

By default, the buffer at each index is `nil`.

## See Also

### Assigning Buffers

func setTileBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the tile shader argument table.

func setTileBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the tile shader argument table.

**Required**

func setTileBufferOffset(Int, index: Int)

Updates an entry in the tile shader argument table with a new location within the entry’s current buffer.

**Required**

