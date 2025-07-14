

- Metal
- MTLRenderCommandEncoder
-  setObjectBuffers(\_:offsets:range:) 

Instance Method

# setObjectBuffers(\_:offsets:range:)

Assigns multiple buffers to a range of entries in the object shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func setObjectBuffers(
    _ buffers: [(any MTLBuffer)?],
    offsets: [Int],
    range: Range
)
```

## Parameters 

`buffers`  

An array of MTLBuffer instances the command assigns to entries in the object shader argument table for buffers.

`offsets`  

An array of integers. Each element represents the location, in bytes, from the start of the corresponding MTLBuffer element in `buffers` where the object shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`range`  

A span of integers that represent the entries in the object shader argument table for buffers. Each entry stores a record of the corresponding element in `buffers` and `offsets`.

## Discussion

By default, the texture at each index is `nil`.

Note

The Objective-C version of this method is setObjectBuffers:offsets:withRange:.

## See Also

### Assigning Buffers for Object Shaders

func setObjectBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the object shader argument table.

**Required**

func setObjectBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the object shader argument table.

**Required**

func setObjectBufferOffset(Int, index: Int)

Updates an entry in the object shader argument table with a new location within the entry’s current buffer.

**Required**

