

- Metal
- MTLDevice
-  makeRenderPipelineState(descriptor:options:) 

Instance Method

# makeRenderPipelineState(descriptor:options:)

Synchronously creates a render pipeline state and reflection information in a tuple.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS

``` source
func makeRenderPipelineState(
    descriptor: MTLRenderPipelineDescriptor,
    options: MTLPipelineOption
) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)
```

## Parameters 

`descriptor`  

An MTLRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

## Return Value

A tuple with a new MTLRenderPipelineState instance and an MTLRenderPipelineReflection optional instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

Use the graphics-rendering pipeline state to configure a render pass by calling the setRenderPipelineState(_:) method of an MTLRenderCommandEncoder instance.

## See Also

### Creating Render Pipeline States with Vertex Shaders

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, completionHandler: MTLNewRenderPipelineStateCompletionHandler)

Asynchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state and reflection information.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a render pipeline state and reflection information.

**Required** Default implementations provided.

