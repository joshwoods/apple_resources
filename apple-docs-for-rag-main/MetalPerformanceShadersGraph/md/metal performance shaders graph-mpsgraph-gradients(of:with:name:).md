

- Metal Performance Shaders Graph
- MPSGraph
-  gradients(of:with:name:) 

Instance Method

# gradients(of:with:name:)

Calculates a partial derivative of primaryTensor with respect to the tensors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func gradients(
    of primaryTensor: MPSGraphTensor,
    with tensors: [MPSGraphTensor],
    name: String?
) -> [MPSGraphTensor : MPSGraphTensor]
```

## Parameters 

`primaryTensor`  

Tensor to be differentiated (numerator).

`tensors`  

Tensors to do the differentiation with (denominator).

`name`  

Name for the gradient operation.

## Return Value

A valid MPSGraphTensor dictionary object containing partial derivative d(primaryTensor)/d(secondaryTensor) for each tensor as key.

