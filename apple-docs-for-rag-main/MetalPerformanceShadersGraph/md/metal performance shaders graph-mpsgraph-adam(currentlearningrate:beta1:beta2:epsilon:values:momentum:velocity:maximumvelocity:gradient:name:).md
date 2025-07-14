

- Metal Performance Shaders Graph
- MPSGraph
-  adam(currentLearningRate:beta1:beta2:epsilon:values:momentum:velocity:maximumVelocity:gradient:name:) 

Instance Method

# adam(currentLearningRate:beta1:beta2:epsilon:values:momentum:velocity:maximumVelocity:gradient:name:)

Creates operations to apply Adam optimization.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func adam(
    currentLearningRate currentLearningRateTensor: MPSGraphTensor,
    beta1 beta1Tensor: MPSGraphTensor,
    beta2 beta2Tensor: MPSGraphTensor,
    epsilon epsilonTensor: MPSGraphTensor,
    values valuesTensor: MPSGraphTensor,
    momentum momentumTensor: MPSGraphTensor,
    velocity velocityTensor: MPSGraphTensor,
    maximumVelocity maximumVelocityTensor: MPSGraphTensor?,
    gradient gradientTensor: MPSGraphTensor,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`beta1Tensor`  

beta1Tensor

`beta2Tensor`  

beta2Tensor

`epsilonTensor`  

Epsilon tensor

`valuesTensor`  

Values to update with optimization

`momentumTensor`  

Momentum tensor

`velocityTensor`  

Velocity tensor

`maximumVelocityTensor`  

Optional maximum velocity tensor

`gradientTensor`  

Partial gradient of the trainable parameters with respect to loss

`name`  

Name for the operation

## Return Value

If maximumVelocity is nil array of 3 tensors (update, newMomentum, newVelocity) else array of 4 tensors (update, newMomentum, newVelocity, newMaximumVelocity)

## Discussion

The adam update ops are added

```
```

