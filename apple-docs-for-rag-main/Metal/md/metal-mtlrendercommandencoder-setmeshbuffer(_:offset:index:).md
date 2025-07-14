

- Metal
- MTLRenderCommandEncoder
-  setMeshBuffer(\_:offset:index:) 

Instance Method

# setMeshBuffer(\_:offset:index:)

Assigns a buffer to an entry in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setMeshBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

An MTLBuffer instance the command assigns to an entry in the mesh shader argument table for buffers.

`offset`  

An integer that represents the location, in bytes, from the start of `buffer` where the mesh shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`index`  

An integer that represents the entry in the mesh shader argument table for buffers that stores a record of `buffer` and `offset`.

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Discussion

By default, the texture at each index is `nil`.

## See Also

### Assigning Buffers for Mesh Shaders

func setMeshBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the mesh shader argument table.

func setMeshBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the mesh shader argument table.

**Required**

func setMeshBufferOffset(Int, index: Int)

Updates an entry in the mesh shader argument table with a new location within the entry’s current buffer.

**Required**

