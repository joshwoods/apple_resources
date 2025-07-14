

- Metal
- MTLRenderCommandEncoder
-  setTileBytes(\_:length:index:) 

Instance Method

# setTileBytes(\_:length:index:)

Creates a buffer from bytes and assigns it to an entry in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setTileBytes(
    _ bytes: UnsafeRawPointer,
    length: Int,
    index: Int
)
```

**Required**

## Parameters 

`bytes`  

A pointer to argument data the method copies to an MTLBuffer and assigns to an entry in the tile shader argument table for buffers.

`length`  

The number of bytes the method copies from the `bytes` pointer.

`index`  

An integer that represents the entry in the tile shader argument table for buffers that stores a record of the MTLBuffer the method creates from `bytes`.

## Discussion

The method is equivalent to creating an MTLBuffer instance that contains the same data as `bytes` and calling the setTileBuffer(_:offset:index:) method. However, this method avoids the overhead of creating a buffer to store your data; instead, Metal manages the data.

Important

Only call this method for single-use data that’s smaller than 4 KB.

For data that’s more than 4 KB, create an MTLBuffer instance and pass it to setTileBuffer(_:offset:index:).

By default, the buffer at each index is `nil`.

## See Also

### Assigning Buffers

func setTileBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the tile shader argument table.

**Required**

func setTileBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the tile shader argument table.

func setTileBufferOffset(Int, index: Int)

Updates an entry in the tile shader argument table with a new location within the entry’s current buffer.

**Required**

