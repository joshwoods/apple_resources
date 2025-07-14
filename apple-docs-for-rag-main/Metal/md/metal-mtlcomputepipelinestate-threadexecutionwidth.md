

- Metal
- MTLComputePipelineState
-  threadExecutionWidth 

Instance Property

# threadExecutionWidth

The number of threads that the GPU executes simultaneously.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var threadExecutionWidth: Int { get }
```

**Required**

## Mentioned in 

Creating Threads and Threadgroups

Calculating Threadgroup and Grid Sizes

## Discussion

For better performance, when dispatching a compute command, make the number of threads in the threadgroup a multiple of `threadExecutionWidth`.

See Creating Threads and Threadgroups and Calculating Threadgroup and Grid Sizes for more information on aligning data, thread width, and threadgroup size.

## See Also

### Checking Threadgroup Attributes

var maxTotalThreadsPerThreadgroup: Int

The maximum number of threads in a threadgroup that you can dispatch to the pipeline.

**Required**

var staticThreadgroupMemoryLength: Int

The length, in bytes, of statically allocated threadgroup memory.

**Required**

