

- ML Compute
- MLCAdamOptimizer
-  init(descriptor:) Deprecated

Initializer

# init(descriptor:)

Creates an Adam optimizer with the descriptor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(descriptor optimizerDescriptor: MLCOptimizerDescriptor)
```

## Parameters 

`optimizerDescriptor`  

An object for configuring the optimizer.

## Return Value

An Adam optimizer.

## Discussion

Sets beta1 to `0.9`, beta2 to `0.999`, epsilon to `1e-8`, usesAMSGrad to `false`, and timeStep to `1` by default.

## See Also

### Creating an Adam Optimizer

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, timeStep: Int)

Creates an Adam optimizer with the values you specify.

Deprecated

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, usesAMSGrad: Bool, timeStep: Int)

Creates an Adam optimizer with the values you specify.

Deprecated

