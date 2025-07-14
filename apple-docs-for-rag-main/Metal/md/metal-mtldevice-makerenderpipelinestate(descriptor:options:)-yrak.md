

- Metal
- MTLDevice
-  makeRenderPipelineState(descriptor:options:) 

Instance Method

# makeRenderPipelineState(descriptor:options:)

Synchronously creates a mesh render pipeline state and reflection information in a tuple.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func makeRenderPipelineState(
    descriptor: MTLMeshRenderPipelineDescriptor,
    options: MTLPipelineOption
) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)
```

## Parameters 

`descriptor`  

An MTLMeshRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

## Return Value

A tuple with a new MTLRenderPipelineState instance and an MTLRenderPipelineReflection optional instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

Use the graphics-rendering pipeline state to configure a render pass by calling the setRenderPipelineState(_:) method of an MTLRenderCommandEncoder instance.

## See Also

### Creating Render Pipeline States with Mesh Shaders

func makeRenderPipelineState(descriptor: MTLMeshRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a mesh render pipeline state and reflection information.

**Required** Default implementations provided.

