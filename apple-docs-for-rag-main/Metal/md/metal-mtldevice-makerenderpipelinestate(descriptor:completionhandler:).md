

- Metal
- MTLDevice
-  makeRenderPipelineState(descriptor:completionHandler:) 

Instance Method

# makeRenderPipelineState(descriptor:completionHandler:)

Asynchronously creates a render pipeline state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeRenderPipelineState(
    descriptor: MTLRenderPipelineDescriptor,
    completionHandler: @escaping MTLNewRenderPipelineStateCompletionHandler
)
```

``` source
func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor) async throws -> any MTLRenderPipelineState
```

**Required**

## Parameters 

`descriptor`  

An MTLRenderPipelineDescriptor instance.

`completionHandler`  

A Swift closure or an Objective-C block the method calls when it finishes creating the render pipeline state.

## Discussion

Use the graphics-rendering pipeline state to configure a render pass by calling the setRenderPipelineState(_:) method of an MTLRenderCommandEncoder instance.

## See Also

### Creating Render Pipeline States with Vertex Shaders

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state and reflection information.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a render pipeline state and reflection information.

**Required** Default implementations provided.

