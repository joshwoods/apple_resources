

- Metal
- MTLRenderPipelineState
-  makeVisibleFunctionTable(descriptor:stage:) 

Instance Method

# makeVisibleFunctionTable(descriptor:stage:)

Creates a new visible function table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func makeVisibleFunctionTable(
    descriptor: MTLVisibleFunctionTableDescriptor,
    stage: MTLRenderStages
) -> (any MTLVisibleFunctionTable)?
```

**Required**

## Parameters 

`descriptor`  

An MTLVisibleFunctionTableDescriptor instance that configures the visible function table the method creates.

`stage`  

An MTLRenderStages instance that represents the render pass stage the visible function table applies to.

## See Also

### Creating Function Handles and Tables

func functionHandle(function: any MTLFunction, stage: MTLRenderStages) -> (any MTLFunctionHandle)?

Creates a function handle for a shader.

**Required**

func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLIntersectionFunctionTable)?

Creates a new intersection function table.

**Required**

