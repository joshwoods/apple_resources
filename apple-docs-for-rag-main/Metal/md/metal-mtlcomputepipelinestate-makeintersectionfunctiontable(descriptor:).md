

- Metal
- MTLComputePipelineState
-  makeIntersectionFunctionTable(descriptor:) 

Instance Method

# makeIntersectionFunctionTable(descriptor:)

Creates a new intersection function table.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor) -> (any MTLIntersectionFunctionTable)?
```

**Required**

## Parameters 

`descriptor`  

An MTLIntersectionFunctionTableDescriptor instance that configures the created table.

## Return Value

A new intersection function table, or `nil` if an error occurred in creation.

## See Also

### Creating Function Tables

func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor) -> (any MTLVisibleFunctionTable)?

Creates a new visible function table.

**Required**

