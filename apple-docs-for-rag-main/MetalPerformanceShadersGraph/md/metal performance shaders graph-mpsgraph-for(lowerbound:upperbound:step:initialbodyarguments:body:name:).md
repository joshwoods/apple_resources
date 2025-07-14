

- Metal Performance Shaders Graph
- MPSGraph
-  for(lowerBound:upperBound:step:initialBodyArguments:body:name:) 

Instance Method

# for(lowerBound:upperBound:step:initialBodyArguments:body:name:)

Adds a for loop operation, The lower and upper bounds specify a half-open range: the range includes the lower bound but does not include the upper bound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func `for`(
    lowerBound: MPSGraphTensor,
    upperBound: MPSGraphTensor,
    step: MPSGraphTensor,
    initialBodyArguments: [MPSGraphTensor],
    body: @escaping MPSGraphForLoopBodyBlock,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`lowerBound`  

Lower bound value of the loop, this is a scalar tensor, this is the index the loop will start with.

`upperBound`  

Upper bound value of the loop, this is a scalar tensor.

`step`  

Step value of the loop, this is a scalar tensor and must be positive.

`initialBodyArguments`  

Initial set of iteration arguments passed to the bodyBlock of the for loop.

`body`  

This block will execute the body of the for loop.

`name`  

Name of operation.

## Return Value

A valid `MPSGraphTensor` array with same count and corresponding element types as `initialIterationArguments` and return types of the for loop.

