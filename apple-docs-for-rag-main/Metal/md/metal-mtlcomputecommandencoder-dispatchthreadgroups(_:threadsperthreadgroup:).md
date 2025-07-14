

- Metal
- MTLComputeCommandEncoder
-  dispatchThreadgroups(\_:threadsPerThreadgroup:) 

Instance Method

# dispatchThreadgroups(\_:threadsPerThreadgroup:)

Encodes a compute dispatch command using a grid aligned to threadgroup boundaries.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func dispatchThreadgroups(
    _ threadgroupsPerGrid: MTLSize,
    threadsPerThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`threadgroupsPerGrid`  

An MTLSize instance that represents the number of threads for each grid dimension.

`threadsPerThreadgroup`  

An MTLSize instance that represents the number of threads in a threadgroup.

## Mentioned in 

Calculating Threadgroup and Grid Sizes

## Discussion

Tip

Prefer using dispatchThreads for your kernel calls on `Apple4` and later Apple GPUs. See Metal Feature Set Tables (PDF) for information on hardware support.

Metal calculates the number of threads in a grid by multiplying `threadsPerThreadgroup` by `threadgroupsPerGrid`.

If the size of your data doesn’t match the size of the grid, perform boundary checks in your compute function to avoid accessing data out of bounds. See Calculating Threadgroup and Grid Sizes for an example.

## See Also

### Dispatching Kernel Calls Directly

func dispatchThreads(MTLSize, threadsPerThreadgroup: MTLSize)

Encodes a compute command using an arbitrarily sized grid.

**Required**

