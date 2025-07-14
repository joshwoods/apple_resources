

- Metal
- MTLRenderPipelineState
-  makeRenderPipelineState(additionalBinaryFunctions:) 

Instance Method

# makeRenderPipelineState(additionalBinaryFunctions:)

Creates a new pipeline state that’s a copy of the current pipeline state with additional shaders.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func makeRenderPipelineState(additionalBinaryFunctions: MTLRenderPipelineFunctionsDescriptor) throws -> any MTLRenderPipelineState
```

**Required**

## Parameters 

`additionalBinaryFunctions`  

An MTLRenderPipelineFunctionsDescriptor instance, which contains MTLFunction arrays for vertex, fragment, and tile shaders.

