

- Metal
- MTLComputeCommandEncoder
-  setBuffer(\_:offset:attributeStride:index:) 

Instance Method

# setBuffer(\_:offset:attributeStride:index:)

Binds a buffer with a stride to the buffer argument table, allowing compute kernels to access its data on the GPU.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func setBuffer(
    _ buffer: any MTLBuffer,
    offset: Int,
    attributeStride stride: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

The MTLBuffer instance to bind to the argument table.

`offset`  

The number of bytes to skip in the buffer before the first element of data.

`stride`  

The number of bytes between the start of one element and the start of the next.

`index`  

The index the buffer binds to in the argument table.

## Discussion

Important

Only call this method when the buffer is part of stageInputDescriptor and has its stride set to MTLBufferLayoutStrideDynamic.

For buffers binding to an argument using the `device` address space, align the offset to the data type’s size. The maximum size for an offset is `16` bytes.

For buffers in the `constant` address space, the minimum alignment depends on the hardware running your app. See the Metal feature set tables (PDF) for information on each Apple GPU family.

Rebinding an already bound buffer causes a Metal error.

## See Also

### Encoding Buffers

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Binds a buffer to the buffer argument table, allowing compute kernels to access its data on the GPU.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Binds multiple buffers to the buffer argument table at once, allowing compute kernels to access their data on the GPU.

func setBuffers([(any MTLBuffer)?], offsets: [Int], attributeStrides: [Int], range: Range&lt;Int>)

Binds multiple buffers with data in stride to the buffer argument table at once, allowing compute kernels to access their data on the GPU.

func setBufferOffset(Int, index: Int)

Changes where the data begins in a buffer already bound to the buffer argument table.

**Required**

func setBufferOffset(offset: Int, attributeStride: Int, index: Int)

Changes where the data begins and the distance between adjacent elements in a buffer already bound to the buffer argument table.

**Required**

