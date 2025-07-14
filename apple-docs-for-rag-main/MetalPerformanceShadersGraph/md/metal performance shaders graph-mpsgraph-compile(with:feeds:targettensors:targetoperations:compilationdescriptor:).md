

- Metal Performance Shaders Graph
- MPSGraph
-  compile(with:feeds:targetTensors:targetOperations:compilationDescriptor:) 

Instance Method

# compile(with:feeds:targetTensors:targetOperations:compilationDescriptor:)

Compiles the graph for the given feeds to returns the target tensor values, ensuring all target operations would be executed.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func compile(
    with device: MPSGraphDevice?,
    feeds: [MPSGraphTensor : MPSGraphShapedType],
    targetTensors: [MPSGraphTensor],
    targetOperations: [MPSGraphOperation]?,
    compilationDescriptor: MPSGraphCompilationDescriptor?
) -> MPSGraphExecutable
```

## Parameters 

`device`  

MPSGraph device to optimize for.

`feeds`  

Feeds dictionary for the placeholder tensors.

`targetTensors`  

Tensors for which the caller wishes MPSGraphTensorData to be returned.

`targetOperations`  

Operations to be completed at the end of the run.

`compilationDescriptor`  

Compilation descriptor to set different compilation parameters.

## Return Value

A valid MPSGraphExecutable object

## Discussion

This call blocks until execution has completed. The compilation descriptor helps specialize the executable returned.

