

- ML Compute
- MLCRMSPropOptimizer
-  epsilon 

Instance Property

# epsilon

The epsilon value you use to improve numerical stability.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
var epsilon: Float { get }
```

## Discussion

The default value is `1e-8`.

## See Also

### Inspecting an RMSProp Optimizer

var momentumScale: Float

A hyper-parameter that specifies the momentum factor.

var alpha: Float

The constant for smoothing.

var isCentered: Bool

A Boolean that indicates whether you compute the centered RMSProp.

