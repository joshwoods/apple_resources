

- Metal Performance Shaders Graph
- MPSGraph
-  stochasticGradientDescent(learningRate:values:gradient:name:) 

Instance Method

# stochasticGradientDescent(learningRate:values:gradient:name:)

The Stochastic gradient descent performs a gradient descent.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func stochasticGradientDescent(
    learningRate learningRateTensor: MPSGraphTensor,
    values valuesTensor: MPSGraphTensor,
    gradient gradientTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`learningRateTensor`  

Scalar tensor which indicates the learning rate to use with the optimizer

`valuesTensor`  

Values tensor, usually representing the trainable parameters

`gradientTensor`  

Partial gradient of the trainable parameters with respect to loss

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

## Discussion

`variable = variable - (learningRate * g)` where, `g` is gradient of error wrt variable

