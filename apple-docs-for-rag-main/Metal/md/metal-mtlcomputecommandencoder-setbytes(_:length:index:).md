

- Metal
- MTLComputeCommandEncoder
-  setBytes(\_:length:index:) 

Instance Method

# setBytes(\_:length:index:)

Copies data directly to the GPU to populate an entry in the buffer argument table.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setBytes(
    _ bytes: UnsafeRawPointer,
    length: Int,
    index: Int
)
```

**Required**

## Parameters 

`bytes`  

A pointer to where the data to copy starts.

`length`  

The number of bytes to copy.

`index`  

The index the data binds to in the argument table.

## Discussion

Important

This method only works for data smaller than 4 kilobytes that doesn’t persist. Create an MTLBuffer instance if your data exceeds 4 KB, needs to persist on the GPU, or you access results on the CPU.

This method allows Metal to copy data efficiently onto the GPU without the need for your own buffer. Binding data directly can improve performance, especially when making many small allocations.

## See Also

### Encoding Raw Bytes

func setBytes(UnsafeRawPointer, length: Int, attributeStride: Int, index: Int)

Copies data with a given stride directly to the GPU to populate an entry in the buffer argument table.

**Required**

