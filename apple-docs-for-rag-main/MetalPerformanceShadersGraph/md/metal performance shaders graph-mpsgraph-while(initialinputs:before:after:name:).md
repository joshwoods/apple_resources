

- Metal Performance Shaders Graph
- MPSGraph
-  while(initialInputs:before:after:name:) 

Instance Method

# while(initialInputs:before:after:name:)

Adds a while loop operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func `while`(
    initialInputs: [MPSGraphTensor],
    before: @escaping MPSGraphWhileBeforeBlock,
    after: @escaping MPSGraphWhileAfterBlock,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`initialInputs`  

inputTensors to the `beforeBlock`, for the 1st iteration will be same as initialInputs passed to the while loop.

`before`  

`beforeBlock`, this will be run first and then call the `afterBlock` with results or return results from the loop.

`after`  

`afterBlock`, this will execute after the condition evaluation.

`name`  

Name of operation.

## Return Value

A valid MPSGraphTensor array with results returned from the conditionBlock depending on the predicate tensor.

