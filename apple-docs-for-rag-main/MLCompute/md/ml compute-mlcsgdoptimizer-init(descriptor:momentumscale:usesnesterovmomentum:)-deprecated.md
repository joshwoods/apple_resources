

- ML Compute
- MLCSGDOptimizer
-  init(descriptor:momentumScale:usesNesterovMomentum:) Deprecated

Initializer

# init(descriptor:momentumScale:usesNesterovMomentum:)

Create an SGD optimizer with the descriptor, momentum scale, and option to enable Nesterov momentum that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    descriptor optimizerDescriptor: MLCOptimizerDescriptor,
    momentumScale: Float,
    usesNesterovMomentum: Bool
)
```

## Parameters 

`optimizerDescriptor`  

An object you use to configure the optimizer.

`momentumScale`  

The momentum scale.

`usesNesterovMomentum`  

A Boolean that indicates whether you enable Nesterov momentum.

## See Also

### Creating an SGD Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an SGD optimizer with the descriptor you specify.

Deprecated

