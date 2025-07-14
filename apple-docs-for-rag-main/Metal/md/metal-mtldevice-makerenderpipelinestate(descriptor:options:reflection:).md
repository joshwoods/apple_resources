

- Metal
- MTLDevice
-  makeRenderPipelineState(descriptor:options:reflection:) 

Instance Method

# makeRenderPipelineState(descriptor:options:reflection:)

Synchronously creates a render pipeline state and reflection information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeRenderPipelineState(
    descriptor: MTLRenderPipelineDescriptor,
    options: MTLPipelineOption,
    reflection: AutoreleasingUnsafeMutablePointer?
) throws -> any MTLRenderPipelineState
```

**Required**

## Parameters 

`descriptor`  

An MTLRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`reflection`  

A pointer to an MTLAutoreleasedRenderPipelineReflection instance.

On return, if the method completes successfully, it fills the instance with the details about the function arguments; otherwise `nil`.

Set to `nil` if you don’t need reflection data.

## Return Value

A new MTLRenderPipelineState instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

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

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a render pipeline state and reflection information.

**Required** Default implementations provided.

