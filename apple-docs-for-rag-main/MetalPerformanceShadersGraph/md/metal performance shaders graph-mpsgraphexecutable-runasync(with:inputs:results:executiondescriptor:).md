

- Metal Performance Shaders Graph
- MPSGraphExecutable
-  runAsync(with:inputs:results:executionDescriptor:) 

Instance Method

# runAsync(with:inputs:results:executionDescriptor:)

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed. This call is asynchronous and will return immediately.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func runAsync(
    with commandQueue: any MTLCommandQueue,
    inputs inputsArray: [MPSGraphTensorData],
    results resultsArray: [MPSGraphTensorData]?,
    executionDescriptor: MPSGraphExecutableExecutionDescriptor?
) -> [MPSGraphTensorData]
```

## Parameters 

`commandQueue`  

CommandQueue passed to exectute the graph on.

`inputsArray`  

Feeds tensorData for the placeholder tensors, same order as arguments of main function.

`resultsArray`  

Tensors for which the caller wishes MPSGraphTensorData to be returned.

`executionDescriptor`  

ExecutionDescriptor to be passed in and used.

## Return Value

A valid MPSGraphTensorData array with results synchronized to the CPU memory if MPSGraphOptionsSynchronizeResults set.

