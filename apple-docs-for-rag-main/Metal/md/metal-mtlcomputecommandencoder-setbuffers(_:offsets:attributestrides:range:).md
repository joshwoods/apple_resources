

- Metal
- MTLComputeCommandEncoder
-  setBuffers(\_:offsets:attributeStrides:range:) 

Instance Method

# setBuffers(\_:offsets:attributeStrides:range:)

Binds multiple buffers with data in stride to the buffer argument table at once, allowing compute kernels to access their data on the GPU.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
func setBuffers(
    _ buffers: [(any MTLBuffer)?],
    offsets: [Int],
    attributeStrides: [Int],
    range: Range
)
```

## Parameters 

`buffers`  

The MTLBuffer instances to bind to the buffer argument table.

`offsets`  

An array of offsets, each of which specifies where the data begins, in bytes, from the start of its corresponding buffer.

`attributeStrides`  

An array of strides, each of which specifies the number of bytes between the start of one element and the start of the next for its corresponding buffer.

`range`  

The argument table indicies to bind each of the `buffers` to, in the order they appear.

## Discussion

Important

This method requires that the length of `buffers`, `offsets`, and `attributeStrides` are all equal to the length of `range`.

For buffers binding to an argument using the `device` address space, align the offset to the data type’s size. The maximum size for an offset is `16` bytes.

For buffers in the `constant` address space, the minimum alignment depends on the hardware running your app. See the Metal feature set tables (PDF) for information on each Apple GPU family.

Rebinding an already bound buffer causes a Metal error.

## See Also

### Encoding Buffers

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Binds a buffer to the buffer argument table, allowing compute kernels to access its data on the GPU.

**Required**

func setBuffer(any MTLBuffer, offset: Int, attributeStride: Int, index: Int)

Binds a buffer with a stride to the buffer argument table, allowing compute kernels to access its data on the GPU.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Binds multiple buffers to the buffer argument table at once, allowing compute kernels to access their data on the GPU.

func setBufferOffset(Int, index: Int)

Changes where the data begins in a buffer already bound to the buffer argument table.

**Required**

func setBufferOffset(offset: Int, attributeStride: Int, index: Int)

Changes where the data begins and the distance between adjacent elements in a buffer already bound to the buffer argument table.

**Required**

