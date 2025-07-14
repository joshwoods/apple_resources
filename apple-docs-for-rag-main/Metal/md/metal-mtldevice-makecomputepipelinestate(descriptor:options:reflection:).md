

- Metal
- MTLDevice
-  makeComputePipelineState(descriptor:options:reflection:) 

Instance Method

# makeComputePipelineState(descriptor:options:reflection:)

Synchronously creates a compute pipeline state and reflection information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func makeComputePipelineState(
    descriptor: MTLComputePipelineDescriptor,
    options: MTLPipelineOption,
    reflection: AutoreleasingUnsafeMutablePointer?
) throws -> any MTLComputePipelineState
```

**Required**

## Parameters 

`descriptor`  

An MTLComputePipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`reflection`  

A pointer to an optional MTLAutoreleasedRenderPipelineReflection instance.

On return, if the method completes successfully, it sets the pointer to an instance with the details about the function arguments; otherwise `nil`.

Set to `nil` if you don’t need reflection data.

## Discussion

Use the compute pipeline state to configure a compute pass by calling the setComputePipelineState(_:) method of an MTLComputeCommandEncoder instance.

## See Also

### Creating Compute Pipeline States

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection information.

**Required** Default implementation provided.

func makeComputePipelineState(function: any MTLFunction) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, completionHandler: MTLNewComputePipelineStateCompletionHandler)

Asynchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedComputePipelineReflection?>?) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state and reflection with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection with a function instance.

**Required**

