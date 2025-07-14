

- ML Compute
- MLCLossDescriptor
-  labelSmoothing Deprecated

Instance Property

# labelSmoothing

The value for label smoothing.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var labelSmoothing: Float { get }
```

## Discussion

The default value is `1.0`.

Note

This is only valid for the following loss function types:

MLCLossType.softmaxCrossEntropy

MLCLossType.sigmoidCrossEntropy

## See Also

### Inspecting Loss Descriptors

var lossType: MLCLossType

The loss function type.

Deprecated

var reductionType: MLCReductionType

The reduction operation performed by the loss function.

Deprecated

var weight: Float

The scale factor you apply to each element of a result.

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

