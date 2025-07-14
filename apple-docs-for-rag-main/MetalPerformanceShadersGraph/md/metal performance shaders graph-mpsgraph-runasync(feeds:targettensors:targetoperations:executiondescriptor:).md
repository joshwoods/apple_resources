

- Metal Performance Shaders Graph
- MPSGraph
-  runAsync(feeds:targetTensors:targetOperations:executionDescriptor:) 

Instance Method

# runAsync(feeds:targetTensors:targetOperations:executionDescriptor:)

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func runAsync(
    feeds: [MPSGraphTensor : MPSGraphTensorData],
    targetTensors: [MPSGraphTensor],
    targetOperations: [MPSGraphOperation]?,
    executionDescriptor: MPSGraphExecutionDescriptor?
) -> [MPSGraphTensor : MPSGraphTensorData]
```

## Parameters 

`feeds`  

Feeds dictionary for the placeholder tensors.

`targetTensors`  

Tensors for which the caller wishes MPSGraphTensorData to be returned.

`targetOperations`  

Operations to be completed at the end of the run.

`executionDescriptor`  

ExecutionDescriptor to be passed in and used.

## Return Value

A valid MPSGraphTensor : MPSGraphTensorData dictionary with results synchronized to the CPU memory.

## Discussion

This call is asynchronous and will return immediately if a completionHandler is set.

