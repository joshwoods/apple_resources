

- Metal Performance Shaders Graph
- MPSGraph
-  encode(to:feeds:targetOperations:resultsDictionary:executionDescriptor:) 

Instance Method

# encode(to:feeds:targetOperations:resultsDictionary:executionDescriptor:)

Encodes the graph for the given feeds to returns the target tensor values in the results dictionary provided by the user.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func encode(
    to commandBuffer: MPSCommandBuffer,
    feeds: [MPSGraphTensor : MPSGraphTensorData],
    targetOperations: [MPSGraphOperation]?,
    resultsDictionary: [MPSGraphTensor : MPSGraphTensorData],
    executionDescriptor: MPSGraphExecutionDescriptor?
)
```

## Parameters 

`commandBuffer`  

commandBuffer passed to execute the graph on, commitAndContinue might be called, please don’t rely on underlying MTLCommandBuffer to remain uncommitted.

`feeds`  

Feeds dictionary for the placeholder tensors.

`targetOperations`  

Operations to be completed at the end of the run.

`resultsDictionary`  

MPSGraphTensors dictionary passed by user, these will be filled with graph output data.

`executionDescriptor`  

ExecutionDescriptor to be passed in and used.

## Discussion

It ensures all target operations also executed. This call is asynchronous and will return immediately if a completionHandler is set.

