

- Metal
- MTLComputePipelineState
-  maxTotalThreadsPerThreadgroup 

Instance Property

# maxTotalThreadsPerThreadgroup

The maximum number of threads in a threadgroup that you can dispatch to the pipeline.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var maxTotalThreadsPerThreadgroup: Int { get }
```

**Required**

## Mentioned in 

Calculating Threadgroup and Grid Sizes

## Discussion

When you create a compute pipeline state, it calculates the maximum number of threads available on the device. This value never changes, but may be different for different pipeline objects.

See Creating Threads and Threadgroups and Calculating Threadgroup and Grid Sizes for more information on aligning data, thread width, and threadgroup size.

## See Also

### Checking Threadgroup Attributes

var threadExecutionWidth: Int

The number of threads that the GPU executes simultaneously.

**Required**

var staticThreadgroupMemoryLength: Int

The length, in bytes, of statically allocated threadgroup memory.

**Required**

