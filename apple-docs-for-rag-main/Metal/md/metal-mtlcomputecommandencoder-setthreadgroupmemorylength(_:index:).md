

- Metal
- MTLComputeCommandEncoder
-  setThreadgroupMemoryLength(\_:index:) 

Instance Method

# setThreadgroupMemoryLength(\_:index:)

Configures the size of a block of threadgroup memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setThreadgroupMemoryLength(
    _ length: Int,
    index: Int
)
```

**Required**

## Parameters 

`length`  

The size of the threadgroup memory, in bytes. Use be a multiple of `16` bytes.

`index`  

The index in the threadgroup memory argument table using this allocation.

## Discussion

Important

The sum of all threadgroup memory allocations (whether made using this method or directly in the shader) can’t exceed the device limits for threadgroup memory. Check threadgroup memory limits with the staticThreadgroupMemoryLength property.

The `threadgroup` memory space allows for sharing data between multiple threads in a threadgroup, which can be faster than using `device` memory in your kernels. Before using any threadgroup memory, call this method to configure the threadgroup memory argument table. Kernels accessing their arguments from threadgroup memory have the `[[threadgroup]]` attribute.

To learn more about using the threadgroup address space, see the Metal Shading Language Specification section 4.4.

## See Also

### Encoding Tile Memory Usage

func setImageblockWidth(Int, height: Int)

Sets the size, in pixels, of imageblock data in tile memory.

**Required**

