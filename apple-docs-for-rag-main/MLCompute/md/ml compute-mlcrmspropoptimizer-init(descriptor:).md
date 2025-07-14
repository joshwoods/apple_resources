

- ML Compute
- MLCRMSPropOptimizer
-  init(descriptor:) 

Initializer

# init(descriptor:)

Creates an RMSProp optimizer with the descriptor you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
convenience init(descriptor optimizerDescriptor: MLCOptimizerDescriptor)
```

## Parameters 

`optimizerDescriptor`  

An object you use to configure the optimizer.

## Return Value

An RMSProp optimizer.

## Discussion

Sets momentumScale to `0.0`, alpha to `0.99`, epsilon to `1e-8` , and isCentered to `false` by default.

## See Also

### Creating an RMSProp Optimizer

convenience init(descriptor: MLCOptimizerDescriptor, momentumScale: Float, alpha: Float, epsilon: Float, isCentered: Bool)

Creates an RMSProp optimizer with the descriptor, momentum scale, smoothing, epsilon, and option to compute the centered RMSProp that you specify.

