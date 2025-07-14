

- Metal
- MTLDevice
-  makeRenderPipelineState(tileDescriptor:options:reflection:) 

Instance Method

# makeRenderPipelineState(tileDescriptor:options:reflection:)

Synchronously creates a tile shader’s render pipeline state and reflection information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func makeRenderPipelineState(
    tileDescriptor descriptor: MTLTileRenderPipelineDescriptor,
    options: MTLPipelineOption,
    reflection: AutoreleasingUnsafeMutablePointer?
) throws -> any MTLRenderPipelineState
```

**Required**

## Parameters 

`descriptor`  

An MTLTileRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`reflection`  

A pointer to an MTLAutoreleasedRenderPipelineReflection instance.

On return, if the method completes successfully, it fills the instance with the details about the function arguments; otherwise `nil`.

Set to `nil` if you don’t need reflection data.

## Return Value

A new MTLRenderPipelineState instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## See Also

### Creating Tile Render Pipeline States

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a tile shader’s render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a tile shader’s render pipeline state and reflection information.

**Required** Default implementation provided.

