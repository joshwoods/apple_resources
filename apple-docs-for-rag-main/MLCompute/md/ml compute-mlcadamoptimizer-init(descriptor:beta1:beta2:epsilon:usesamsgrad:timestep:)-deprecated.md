

- ML Compute
- MLCAdamOptimizer
-  init(descriptor:beta1:beta2:epsilon:usesAMSGrad:timeStep:) Deprecated

Initializer

# init(descriptor:beta1:beta2:epsilon:usesAMSGrad:timeStep:)

Creates an Adam optimizer with the values you specify.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
convenience init(
    descriptor optimizerDescriptor: MLCOptimizerDescriptor,
    beta1: Float,
    beta2: Float,
    epsilon: Float,
    usesAMSGrad: Bool,
    timeStep: Int
)
```

## Parameters 

`optimizerDescriptor`  

An object for configuring the optimizer.

`beta1`  

The coefficent for computing running averages of gradient. The default value is `0.9`.

`beta2`  

The coefficent for computing running averages of square of gradient. The default value is `0.999`.

`epsilon`  

The epsilon value for improving numerical stability. The default value is `1e-8`.

`usesAMSGrad`  

A Boolean that indicates whether to use a variant of the algorithm. The default value is `false`.

`timeStep`  

The initial timestep for the update. The default value is `1`.

## See Also

### Creating an Adam Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an Adam optimizer with the descriptor you specify.

Deprecated

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, timeStep: Int)

Creates an Adam optimizer with the values you specify.

Deprecated

