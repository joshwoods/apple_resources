

- Metal Performance Shaders Graph
- MPSGraph
-  applyStochasticGradientDescent(learningRate:variable:gradient:name:) 

Instance Method

# applyStochasticGradientDescent(learningRate:variable:gradient:name:)

The Stochastic gradient descent performs a gradient descent `variable = variable - (learningRate * g)` where, `g` is gradient of error wrt variable this op directly writes to the variable

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func applyStochasticGradientDescent(
    learningRate learningRateTensor: MPSGraphTensor,
    variable: MPSGraphVariableOp,
    gradient gradientTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphOperation
```

## Parameters 

`learningRateTensor`  

Scalar tensor which indicates the learning rate to use with the optimizer

`variable`  

Variable operation with trainable parameters

`gradientTensor`  

Partial gradient of the trainable parameters with respect to loss

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

