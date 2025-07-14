

- Metal
- MTLComputeCommandEncoder
-  setImageblockWidth(\_:height:) 

Instance Method

# setImageblockWidth(\_:height:)

Sets the size, in pixels, of imageblock data in tile memory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setImageblockWidth(
    _ width: Int,
    height: Int
)
```

**Required**

## Parameters 

`width`  

The width of the imageblock, in pixels.

`height`  

The height of the imageblock, in pixels.

## Discussion

Important

The sum of all threadgroup memory allocations (whether made using this method or directly in the shader) can’t exceed the device limits for threadgroup memory. Check threadgroup memory limits with the staticThreadgroupMemoryLength property.

Both imageblocks and threadgroup memory share the available space you can reserve in tile memory, so the sum of these allocations can’t exceed the maximum total tile memory limit. To find the amount of memory used by an imageblock, call imageblockMemoryLength(forDimensions:). Kernels accessing an imageblock argument from threadgroup memory have the `[[threadgroup_imageblock]]` attribute.

To learn more about using imageblocks, see the following sections in the Metal Shading Language Specification:

- For information on the `threadgroup_imageblock` address space, see Section 4.5.

- For information on the `imageblock` type, see Section 2.11.

## See Also

### Encoding Tile Memory Usage

func setThreadgroupMemoryLength(Int, index: Int)

Configures the size of a block of threadgroup memory.

**Required**

