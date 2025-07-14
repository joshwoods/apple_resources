

- Metal
- MTLComputePipelineDescriptor
-  computeFunction 

Instance Property

# computeFunction

The compute kernel the pipeline calls.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var computeFunction: (any MTLFunction)? { get set }
```

## Discussion

Warning

Ensure that this value is non-`nil` before creating a new MTLComputePipelineState with the associated pipeline descriptor instance.

The default value is `nil`.

## See Also

### Configuring the Compute Execution Environment

var threadGroupSizeIsMultipleOfThreadExecutionWidth: Bool

A Boolean value that indicates whether the threadgroup size is always a multiple of the thread execution width.

var maxTotalThreadsPerThreadgroup: Int

The maximum number of threads in a threadgroup that you can dispatch to the compute function.

var maxCallStackDepth: Int

The maximum recursive call depth for dynamic library, visible, and intersection functions.

