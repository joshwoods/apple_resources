

- Metal
- MTLDevice
-  makeRenderPipelineState(tileDescriptor:options:) 

Instance Method

# makeRenderPipelineState(tileDescriptor:options:)

Synchronously creates a tile shader’s render pipeline state and reflection information in a tuple.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS

``` source
func makeRenderPipelineState(
    tileDescriptor: MTLTileRenderPipelineDescriptor,
    options: MTLPipelineOption
) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)
```

## Parameters 

`tileDescriptor`  

An MTLTileRenderPipelineDescriptor instance.

`options`  

An MTLPipelineOption instance that represents the reflection information you want the method to generate.

## Return Value

A tuple with a new MTLTileRenderPipelineDescriptor instance and an MTLRenderPipelineReflection optional instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## See Also

### Creating Tile Render Pipeline States

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a tile shader’s render pipeline state and reflection information.

**Required**

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a tile shader’s render pipeline state and reflection information.

**Required** Default implementation provided.

