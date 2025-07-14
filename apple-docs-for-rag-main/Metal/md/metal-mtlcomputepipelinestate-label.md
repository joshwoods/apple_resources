

- Metal
- MTLComputePipelineState
-  label 

Instance Property

# label

A string that helps you identify the compute pipeline state during debugging.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var label: String? { get }
```

**Required**

## Discussion

Labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying a Pipeline State

var device: any MTLDevice

The device instance that created the pipeline state.

**Required**

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

