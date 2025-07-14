

- ML Compute
- MLCRMSPropOptimizer
-  alpha 

Instance Property

# alpha

The constant for smoothing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
var alpha: Float { get }
```

## Discussion

The default value is `0.99`.

## See Also

### Inspecting an RMSProp Optimizer

var momentumScale: Float

A hyper-parameter that specifies the momentum factor.

var epsilon: Float

The epsilon value you use to improve numerical stability.

var isCentered: Bool

A Boolean that indicates whether you compute the centered RMSProp.

