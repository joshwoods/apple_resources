

- Metal
- MTLComputePipelineState
-  makeVisibleFunctionTable(descriptor:) 

Instance Method

# makeVisibleFunctionTable(descriptor:)

Creates a new visible function table.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor) -> (any MTLVisibleFunctionTable)?
```

**Required**

## Parameters 

`descriptor`  

An MTLVisibleFunctionTableDescriptor instance that configures the created table.

## Return Value

A new visible function table, or `nil` if an error occurred in creation.

## See Also

### Creating Function Tables

func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor) -> (any MTLIntersectionFunctionTable)?

Creates a new intersection function table.

**Required**

