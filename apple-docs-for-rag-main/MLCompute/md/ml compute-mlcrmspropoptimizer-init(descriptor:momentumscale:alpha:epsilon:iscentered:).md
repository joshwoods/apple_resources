

- ML Compute
- MLCRMSPropOptimizer
-  init(descriptor:momentumScale:alpha:epsilon:isCentered:) 

Initializer

# init(descriptor:momentumScale:alpha:epsilon:isCentered:)

Creates an RMSProp optimizer with the descriptor, momentum scale, smoothing, epsilon, and option to compute the centered RMSProp that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
convenience init(
    descriptor optimizerDescriptor: MLCOptimizerDescriptor,
    momentumScale: Float,
    alpha: Float,
    epsilon: Float,
    isCentered: Bool
)
```

## Parameters 

`optimizerDescriptor`  

An object you use to configure the optimizer.

`momentumScale`  

The momentum scale.

`alpha`  

The smoothing constant value.

`epsilon`  

The epsilon value you use to improve numerical stability.

`isCentered`  

A Boolean that indicates whether you compute the centered RMSProp.

## See Also

### Creating an RMSProp Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an RMSProp optimizer with the descriptor you specify.

