

- ML Compute
- MLCLossDescriptor
-  classCount Deprecated

Instance Property

# classCount

The number of classes.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var classCount: Int { get }
```

## Discussion

The default value is 1.

Note

This is only valid for the loss function type MLCLossType.softmaxCrossEntropy.

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

var labelSmoothing: Float

The value for label smoothing.

Deprecated

var epsilon: Float

The epsilon value.

Deprecated

var delta: Float

The delta value.

Deprecated

