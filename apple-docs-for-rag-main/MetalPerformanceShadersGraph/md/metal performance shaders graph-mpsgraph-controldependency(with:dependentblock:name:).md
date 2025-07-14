

- Metal Performance Shaders Graph
- MPSGraph
-  controlDependency(with:dependentBlock:name:) 

Instance Method

# controlDependency(with:dependentBlock:name:)

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func controlDependency(
    with operations: [MPSGraphOperation],
    dependentBlock: @escaping MPSGraphControlFlowDependencyBlock,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`operations`  

Operations maked as control dependency for all ops created inside the dependent block

`dependentBlock`  

MPSGraphControlFlowDependencyBlock which is provided by caller to create dependent ops

`name`  

Name of scope

## Return Value

A valid MPSGraphTensor array with results returned from dependentBlock forwarded

## Discussion

This call blocks until execution has completed.

