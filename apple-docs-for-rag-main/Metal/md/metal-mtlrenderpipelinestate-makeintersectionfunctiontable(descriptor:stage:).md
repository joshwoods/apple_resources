

- Metal
- MTLRenderPipelineState
-  makeIntersectionFunctionTable(descriptor:stage:) 

Instance Method

# makeIntersectionFunctionTable(descriptor:stage:)

Creates a new intersection function table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func makeIntersectionFunctionTable(
    descriptor: MTLIntersectionFunctionTableDescriptor,
    stage: MTLRenderStages
) -> (any MTLIntersectionFunctionTable)?
```

**Required**

## Parameters 

`descriptor`  

An MTLIntersectionFunctionTableDescriptor instance that configures the visible function table the method creates.

`stage`  

An MTLRenderStages instance that represents the render pass stage the intersection function table applies to.

## See Also

### Creating Function Handles and Tables

func functionHandle(function: any MTLFunction, stage: MTLRenderStages) -> (any MTLFunctionHandle)?

Creates a function handle for a shader.

**Required**

func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLVisibleFunctionTable)?

Creates a new visible function table.

**Required**

