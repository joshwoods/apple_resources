

- Metal
- MTLRenderPipelineState
-  functionHandle(function:stage:) 

Instance Method

# functionHandle(function:stage:)

Creates a function handle for a shader.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func functionHandle(
    function: any MTLFunction,
    stage: MTLRenderStages
) -> (any MTLFunctionHandle)?
```

**Required**

## Parameters 

`function`  

An MTLFunction instance that represents the shader the method creates a handle for.

`stage`  

An MTLRenderStages instance that represents the rendering stage that invokes the shader that `function` represents.

## See Also

### Creating Function Handles and Tables

func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLVisibleFunctionTable)?

Creates a new visible function table.

**Required**

func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLIntersectionFunctionTable)?

Creates a new intersection function table.

**Required**

