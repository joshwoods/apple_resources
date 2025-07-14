

- ML Compute
- MLCLossDescriptor
-  weight Deprecated

Instance Property

# weight

The scale factor you apply to each element of a result.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var weight: Float { get }
```

## Discussion

The default value is `1.0`.

## See Also

### Inspecting Loss Descriptors

var lossType: MLCLossType

The loss function type.

Deprecated

var reductionType: MLCReductionType

The reduction operation performed by the loss function.

Deprecated

var labelSmoothing: Float

The value for label smoothing.

Deprecated

var classCount: Int

The number of classes.

Deprecated

var epsilon: Float

The epsilon value.

Deprecated

var delta: Float

The delta value.

Deprecated

