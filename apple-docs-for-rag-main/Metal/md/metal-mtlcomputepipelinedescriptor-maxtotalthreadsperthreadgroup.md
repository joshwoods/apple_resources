

- Metal
- MTLComputePipelineDescriptor
-  maxTotalThreadsPerThreadgroup 

Instance Property

# maxTotalThreadsPerThreadgroup

The maximum number of threads in a threadgroup that you can dispatch to the compute function.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var maxTotalThreadsPerThreadgroup: Int { get set }
```

## Discussion

Important

Both the Metal API and Metal Shader language allow setting the maximum number of threads per threadgroup. When you use both, the value of this property needs to be identical to your shader’s `[[max_total_threads_per_threadgroup]]` attribute, or an error occurs.

By default, when you create an MTLComputePipelineState instance, Metal calculates the maximum number of threads per threadgroup that you can dispatch to it. The MTLDevice and compute pass’s use of memory determine the thread limit. Metal keeps the GPU as saturated as possible, but may use fewer threads in a threadgroup than the maximum.

The maximum number of threads Metal can use in a compute pass is the maxTotalThreadsPerThreadgroup property of the MTLComputePipelineState created from your descriptor.

Metal may return an error if this value is above the total amount of available resources, or could create a compute pipeline state with poor performance.

Profile your app to determine if setting this value is necessary to improve performance. See Analyzing the performance of your Metal app for information on performance profiling.

When this value is `0`, the resulting Metal pipeline determines maximum threadgroup usage automatically.

## See Also

### Configuring the Compute Execution Environment

var computeFunction: (any MTLFunction)?

The compute kernel the pipeline calls.

var threadGroupSizeIsMultipleOfThreadExecutionWidth: Bool

A Boolean value that indicates whether the threadgroup size is always a multiple of the thread execution width.

var maxCallStackDepth: Int

The maximum recursive call depth for dynamic library, visible, and intersection functions.

