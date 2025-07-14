

- Metal
- MTLDevice
-  makeRenderPipelineState(tileDescriptor:options:completionHandler:) 

Instance Method

# makeRenderPipelineState(tileDescriptor:options:completionHandler:)

Asynchronously creates a tile shader’s render pipeline state and reflection information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func makeRenderPipelineState(
    tileDescriptor descriptor: MTLTileRenderPipelineDescriptor,
    options: MTLPipelineOption,
    completionHandler: @escaping MTLNewRenderPipelineStateWithReflectionCompletionHandler
)
```

``` source
func makeRenderPipelineState(
    tileDescriptor descriptor: MTLTileRenderPipelineDescriptor,
    options: MTLPipelineOption
) async throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)
```

**Required** Default implementation provided.

## Parameters 

`descriptor`  

An MTLTileRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

`completionHandler`  

A Swift closure or an Objective-C block the method calls when it finishes creating the render pipeline state.

## Default Implementations

### MTLDevice Implementations

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a tile shader’s render pipeline state and reflection information in a tuple.

## See Also

### Creating Tile Render Pipeline States

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a tile shader’s render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a tile shader’s render pipeline state and reflection information.

**Required**

