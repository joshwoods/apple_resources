

- Metal
- MTLRenderCommandEncoder
-  setMeshBufferOffset(\_:index:) 

Instance Method

# setMeshBufferOffset(\_:index:)

Updates an entry in the mesh shader argument table with a new location within the entry’s current buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setMeshBufferOffset(
    _ offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`offset`  

An integer that represents the location, in bytes, from the start of `buffer` where the mesh shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`index`  

An integer that represents the entry in the mesh shader argument table for buffers that already stores a record of an MTLBuffer.

## Discussion

The command this method encodes changes the offset for a mesh buffer that already has a previous assignment from one of your earlier commands.

For more information, see:

- setMeshBuffer(_:offset:index:)

- setMeshBuffers(_:offsets:range:) (Swift)

- setMeshBuffers:offsets:withRange: (Objective-C)

The command can also adjust the offset for an entry that you previously set with the setMeshBytes(_:length:index:) method.

Tip

If you’re only updating an offset, this method is typically more efficient than rebinding a buffer or byte block with the methods above.

## See Also

### Assigning Buffers for Mesh Shaders

func setMeshBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the mesh shader argument table.

**Required**

func setMeshBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the mesh shader argument table.

func setMeshBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the mesh shader argument table.

**Required**

