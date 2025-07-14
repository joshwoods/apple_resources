

- Metal
- MTLComputeCommandEncoder
-  setComputePipelineState(\_:) 

Instance Method

# setComputePipelineState(\_:)

Configures the compute encoder with a pipeline state instance for subsequent kernel calls.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setComputePipelineState(_ state: any MTLComputePipelineState)
```

**Required**

## Parameters 

`state`  

An MTLComputePipelineState instance.

## Discussion

Important

Set a compute encoder’s pipeline state before encoding any commands. Encoding commands without an available pipeline state causes an error.

Create your pipeline state through one of the MTLDevice methods in Creating Compute Pipeline States.

A compute pipeline state provides information Metal uses to compile and run encoded commands. You can change the pipeline state at any time, allowing you to encode multiple kernel calls in a single command buffer. Changing the pipeline state doesn’t affect any previously encoded commands.

## See Also

### Configuring the Pipeline State

var dispatchType: MTLDispatchType

The dispatch type to use when submitting compute work to the GPU.

**Required**

