

- ML Compute
- MLCRMSPropOptimizer
-  isCentered 

Instance Property

# isCentered

A Boolean that indicates whether you compute the centered RMSProp.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
var isCentered: Bool { get }
```

## Discussion

If `true`, the optimizer normalizes the gradient by an estimation of its variance. The default value is `false`.

## See Also

### Inspecting an RMSProp Optimizer

var momentumScale: Float

A hyper-parameter that specifies the momentum factor.

var alpha: Float

The constant for smoothing.

var epsilon: Float

The epsilon value you use to improve numerical stability.

