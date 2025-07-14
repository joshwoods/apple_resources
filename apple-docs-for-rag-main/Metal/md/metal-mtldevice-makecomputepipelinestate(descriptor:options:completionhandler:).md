

- Metal
- MTLDevice
-  makeComputePipelineState(descriptor:options:completionHandler:) 

Instance Method

# makeComputePipelineState(descriptor:options:completionHandler:)

Asynchronously creates a compute pipeline state and reflection information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func makeComputePipelineState(
    descriptor: MTLComputePipelineDescriptor,
    options: MTLPipelineOption,
    completionHandler: @escaping MTLNewComputePipelineStateWithReflectionCompletionHandler
)
```

``` source
func makeComputePipelineState(
    descriptor: MTLComputePipelineDescriptor,
    options: MTLPipelineOption
) async throws -> (any MTLComputePipelineState, MTLComputePipelineReflection?)
```

**Required** Default implementation provided.

## Parameters 

`descriptor`  

An MTLComputePipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`completionHandler`  

A Swift closure or an Objective-C block the method calls when it finishes creating the compute pipeline state.

## Discussion

Use the compute pipeline state to configure a compute pass by calling the setComputePipelineState(_:) method of an MTLComputeCommandEncoder instance.

## Default Implementations

### MTLDevice Implementations

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLComputePipelineState, MTLComputePipelineReflection?)

## See Also

### Creating Compute Pipeline States

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedComputePipelineReflection?>?) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state and reflection information.

**Required**

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

