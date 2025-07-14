

- Metal
- MTLRenderCommandEncoder
-  setFragmentBufferOffset(\_:index:) 

Instance Method

# setFragmentBufferOffset(\_:index:)

Updates an entry in the fragment shader argument table with a new location within the entry’s current buffer.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setFragmentBufferOffset(
    _ offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`offset`  

An integer that represents the location, in bytes, from the start of `buffer` where the fragment shader argument data begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`index`  

An integer that represents the entry in the fragment shader argument table for buffers that already stores a record of an MTLBuffer.

## Discussion

The command this method encodes changes the offset for a fragment buffer that already has a previous assignment from one of your earlier commands.

For more information, see:

- setFragmentBuffer(_:offset:index:)

- setFragmentBuffers(_:offsets:range:) (Swift)

- setFragmentBuffers:offsets:withRange: (Objective-C)

The command can also adjust the offset for an entry that you previously set with the setFragmentBytes(_:length:index:) method.

Tip

If you’re only updating an offset, this method is typically more efficient than rebinding a buffer or byte block with the methods above.

By default, the buffer at each index is `nil`.

## See Also

### Assigning Buffers

func setFragmentBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the fragment shader argument table.

**Required**

func setFragmentBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the fragment shader argument table.

func setFragmentBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the fragment shader argument table.

**Required**

