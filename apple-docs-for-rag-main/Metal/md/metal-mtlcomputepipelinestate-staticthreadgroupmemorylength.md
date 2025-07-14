

- Metal
- MTLComputePipelineState
-  staticThreadgroupMemoryLength 

Instance Property

# staticThreadgroupMemoryLength

The length, in bytes, of statically allocated threadgroup memory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var staticThreadgroupMemoryLength: Int { get }
```

**Required**

## See Also

### Checking Threadgroup Attributes

var maxTotalThreadsPerThreadgroup: Int

The maximum number of threads in a threadgroup that you can dispatch to the pipeline.

**Required**

var threadExecutionWidth: Int

The number of threads that the GPU executes simultaneously.

**Required**

