

- ML Compute
- MLCAdamWOptimizer
-  init(descriptor:) Deprecated

Initializer

# init(descriptor:)

Creates a default optimizer with the descriptor you specify.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
convenience init(descriptor optimizerDescriptor: MLCOptimizerDescriptor)
```

## Parameters 

`optimizerDescriptor`  

An object for configuring the optimizer.

## Return Value

An AdamW optimizer.

## Discussion

Sets beta1 to `0.9`, beta2 to `0.999`, epsilon to `1e-8`, usesAMSGrad to `false`, and timeStep to `1` by default.

## See Also

### Creating an AdamW Optimizer

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, usesAMSGrad: Bool, timeStep: Int)

Creates an AdamW optimizer with the values you specify.

Deprecated

