

- Metal
- MTLRenderCommandEncoder
-  setVertexBuffer(\_:offset:index:) 

Instance Method

# setVertexBuffer(\_:offset:index:)

Assigns a buffer to an entry in the vertex shader argument table.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setVertexBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

An MTLBuffer instance the command assigns to an entry in the vertex shader argument table for buffers.

`offset`  

An integer that represents the location, in bytes, from the start of `buffer` where the vertex shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`index`  

An integer that represents the entry in the vertex shader argument table for buffers that stores a record of `buffer` and `offset`.

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Discussion

By default, the buffer at each index is `nil`.

## See Also

### Assigning Buffers

func setVertexBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the vertex shader argument table.

func setVertexBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the vertex shader argument table.

**Required**

func setVertexBufferOffset(Int, index: Int)

Updates an entry in the vertex shader argument table with a new location within the entry’s current buffer.

**Required**

