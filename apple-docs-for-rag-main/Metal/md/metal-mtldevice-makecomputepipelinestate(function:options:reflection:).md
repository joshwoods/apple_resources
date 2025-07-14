

- Metal
- MTLDevice
-  makeComputePipelineState(function:options:reflection:) 

Instance Method

# makeComputePipelineState(function:options:reflection:)

Synchronously creates a compute pipeline state and reflection with a function instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeComputePipelineState(
    function computeFunction: any MTLFunction,
    options: MTLPipelineOption,
    reflection: AutoreleasingUnsafeMutablePointer?
) throws -> any MTLComputePipelineState
```

**Required**

## Parameters 

`computeFunction`  

An MTLFunction instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`reflection`  

A pointer to an MTLAutoreleasedRenderPipelineReflection instance. On return, if the method completes successfully, it fills the instance with the details about the function arguments; otherwise `nil`.

Set to `nil` if you don’t need reflection data.

## Discussion

Use the compute pipeline state to configure a compute pass by calling the setComputePipelineState(_:) method of an MTLComputeCommandEncoder instance.

## See Also

### Creating Compute Pipeline States

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedComputePipelineReflection?>?) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state and reflection information.

**Required**

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection information.

**Required** Default implementation provided.

func makeComputePipelineState(function: any MTLFunction) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, completionHandler: MTLNewComputePipelineStateCompletionHandler)

Asynchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection with a function instance.

**Required**

