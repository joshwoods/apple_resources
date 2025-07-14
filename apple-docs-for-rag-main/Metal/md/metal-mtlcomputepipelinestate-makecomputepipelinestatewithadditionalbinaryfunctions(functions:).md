

- Metal
- MTLComputePipelineState
-  makeComputePipelineStateWithAdditionalBinaryFunctions(functions:) 

Instance Method

# makeComputePipelineStateWithAdditionalBinaryFunctions(functions:)

Creates a new pipeline state object with additional callable functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeComputePipelineStateWithAdditionalBinaryFunctions(functions: [any MTLFunction]) throws -> any MTLComputePipelineState
```

**Required**

## Parameters 

`functions`  

The list of additional functions that you want to be able to call.

## Return Value

A new compute pipeline state with access to the provided functions. When this value is `nil`, an error occurred during handle creation.

