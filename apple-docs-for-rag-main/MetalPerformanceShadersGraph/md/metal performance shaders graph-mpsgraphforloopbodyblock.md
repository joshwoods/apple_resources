

- Metal Performance Shaders Graph
-  MPSGraphForLoopBodyBlock 

Type Alias

# MPSGraphForLoopBodyBlock

A block for the body in the for loop.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias MPSGraphForLoopBodyBlock = (MPSGraphTensor, [MPSGraphTensor]) -> [MPSGraphTensor]
```

## Parameters 

`index`  

The for loop index per iteration, it is a scalar tensor.

`iterationArguments`  

Arguments for this iteration, with the same count and corresponding element types as `initialIterationArguments` and return types of the `for` loop.

## Return Value

A valid MPSGraphTensor array with same count and corresponding element types as `initialIterationArguments` and return types of the `for` loop.

