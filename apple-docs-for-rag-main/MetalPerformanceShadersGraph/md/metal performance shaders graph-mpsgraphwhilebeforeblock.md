

- Metal Performance Shaders Graph
-  MPSGraphWhileBeforeBlock 

Type Alias

# MPSGraphWhileBeforeBlock

The block that executes before the condition evaluates for each iteration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias MPSGraphWhileBeforeBlock = ([MPSGraphTensor], NSMutableArray) -> MPSGraphTensor
```

## Parameters 

`inputTensors`  

Input tensors to the `whileConditionBlock`, for the first iteration will be same as initialInputs passed to the while loop.

`resultTensors`  

A valid `MPSGraphTensor` array with results forwarded to after block or returned from the while loop depending on the predicate tensor. It will be empty and the caller block should fill it up before returning.

## Return Value

Tensor MUST be set and have a single scalar value, used to decide between executing the body block or returning from the while loop.

