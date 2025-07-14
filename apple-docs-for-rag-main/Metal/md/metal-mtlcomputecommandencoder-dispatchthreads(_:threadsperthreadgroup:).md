

- Metal
- MTLComputeCommandEncoder
-  dispatchThreads(\_:threadsPerThreadgroup:) 

Instance Method

# dispatchThreads(\_:threadsPerThreadgroup:)

Encodes a compute command using an arbitrarily sized grid.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 14.5+visionOS 1.0+

``` source
func dispatchThreads(
    _ threadsPerGrid: MTLSize,
    threadsPerThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`threadsPerGrid`  

The number of threads in the grid, in each dimension.

`threadsPerThreadgroup`  

The number of threads in one threadgroup, in each dimension.

## Mentioned in 

Calculating Threadgroup and Grid Sizes

## Discussion

Warning

Use this method only if the device your app is running on supports nonuniform threadgroup sizes. Check for device capabilities with supportsFamily(_:) on the device providing your compute command encoder. See Metal Feature Set Tables (PDF) for device support information.

This method encodes a call that uses an arbitrary number of threads in its execution grid. Metal calculates the number of threadgroups needed, providing partial threadgroups if necessary. Prefer this method to dispatchThreadgroups(_:threadsPerThreadgroup:) if your app requires bounds checking or you need extra data allocations to saturate a uniform grid.

## See Also

### Dispatching Kernel Calls Directly

func dispatchThreadgroups(MTLSize, threadsPerThreadgroup: MTLSize)

Encodes a compute dispatch command using a grid aligned to threadgroup boundaries.

**Required**

