

- Metal
- MTLDevice
-  makeRenderPipelineState(descriptor:options:completionHandler:) 

Instance Method

# makeRenderPipelineState(descriptor:options:completionHandler:)

Asynchronously creates a render pipeline state and reflection information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeRenderPipelineState(
    descriptor: MTLRenderPipelineDescriptor,
    options: MTLPipelineOption,
    completionHandler: @escaping MTLNewRenderPipelineStateWithReflectionCompletionHandler
)
```

``` source
func makeRenderPipelineState(
    descriptor: MTLRenderPipelineDescriptor,
    options: MTLPipelineOption
) async throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)
```

**Required** Default implementations provided.

## Parameters 

`descriptor`  

An MTLRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`completionHandler`  

A Swift closure or an Objective-C block the method calls when it finishes creating the render pipeline state.

## Discussion

Use the graphics-rendering pipeline state to configure a render pass by calling the setRenderPipelineState(_:) method of an MTLRenderCommandEncoder instance.

## Default Implementations

### MTLDevice Implementations

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLMeshRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a mesh render pipeline state and reflection information in a tuple.

## See Also

### Creating Render Pipeline States with Vertex Shaders

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, completionHandler: MTLNewRenderPipelineStateCompletionHandler)

Asynchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state and reflection information.

**Required**

