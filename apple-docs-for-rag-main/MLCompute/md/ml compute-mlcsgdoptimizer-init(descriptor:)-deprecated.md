

- ML Compute
- MLCSGDOptimizer
-  init(descriptor:) Deprecated

Initializer

# init(descriptor:)

Creates an SGD optimizer with the descriptor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(descriptor optimizerDescriptor: MLCOptimizerDescriptor)
```

## Parameters 

`optimizerDescriptor`  

An object you use to configure the optimizer.

## Return Value

An SGD optimizer.

## Discussion

Sets momentumScale to `0.0` and usesNesterovMomentum to `false` by default.

## See Also

### Creating an SGD Optimizer

convenience init(descriptor: MLCOptimizerDescriptor, momentumScale: Float, usesNesterovMomentum: Bool)

Create an SGD optimizer with the descriptor, momentum scale, and option to enable Nesterov momentum that you specify.

Deprecated

