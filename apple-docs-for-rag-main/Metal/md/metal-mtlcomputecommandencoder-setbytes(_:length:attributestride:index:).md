

- Metal
- MTLComputeCommandEncoder
-  setBytes(\_:length:attributeStride:index:) 

Instance Method

# setBytes(\_:length:attributeStride:index:)

Copies data with a given stride directly to the GPU to populate an entry in the buffer argument table.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func setBytes(
    _ bytes: UnsafeRawPointer,
    length: Int,
    attributeStride stride: Int,
    index: Int
)
```

**Required**

## Parameters 

`bytes`  

A pointer to the memory where the data to copy starts.

`length`  

The number of bytes to copy.

`stride`  

The number of bytes between the start of one element and the start of the next.

`index`  

The index the data binds to in the argument table.

## Discussion

Important

This method only works for data smaller than 4 kilobytes that doesn’t persist. Create an MTLBuffer instance if your data exceeds 4 KB, needs to persist on the GPU, or you access results on the CPU.

This method allows Metal to copy data directly onto the GPU, rather than creating a new MTLBuffer instance and binding it. Binding data directly can improve performance, especially when making many small allocations.

## See Also

### Encoding Raw Bytes

func setBytes(UnsafeRawPointer, length: Int, index: Int)

Copies data directly to the GPU to populate an entry in the buffer argument table.

**Required**

