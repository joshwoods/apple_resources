

- Metal
- MTLComputePipelineState
-  functionHandle(function:) 

Instance Method

# functionHandle(function:)

Creates a function handle for a visible function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func functionHandle(function: any MTLFunction) -> (any MTLFunctionHandle)?
```

**Required**

## Parameters 

`function`  

An MTLFunction instance that represents the visible function to create a handle for.

## Return Value

A handle to the visible function. When this value is `nil`, an error occurred during handle creation.

