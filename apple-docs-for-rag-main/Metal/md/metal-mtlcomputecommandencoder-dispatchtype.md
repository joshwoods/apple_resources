

- Metal
- MTLComputeCommandEncoder
-  dispatchType 

Instance Property

# dispatchType

The dispatch type to use when submitting compute work to the GPU.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var dispatchType: MTLDispatchType { get }
```

**Required**

## Discussion

You set this property when you create the command encoder, and it doesn’t change for the remainder of the encoding.

See makeComputeCommandEncoder(dispatchType:) for more information.

## See Also

### Configuring the Pipeline State

func setComputePipelineState(any MTLComputePipelineState)

Configures the compute encoder with a pipeline state instance for subsequent kernel calls.

**Required**

