

- ML Compute
-  MLCLossDescriptor Deprecated

Class

# MLCLossDescriptor

A configuration object you use to create a loss layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLossDescriptor
```

## Topics

### Creating Loss Descriptors

convenience init(type: MLCLossType, reductionType: MLCReductionType)

Creates a loss descriptor with the loss function and reduction type you specify.

convenience init(type: MLCLossType, reductionType: MLCReductionType, weight: Float)

Creates a loss descriptor with the loss function, reduction type, and weight you specify.

convenience init(type: MLCLossType, reductionType: MLCReductionType, weight: Float, labelSmoothing: Float, classCount: Int)

Creates a loss descriptor with the loss function, reduction type, weight, label smoothing, and number of classes you specify.

convenience init(type: MLCLossType, reductionType: MLCReductionType, weight: Float, labelSmoothing: Float, classCount: Int, epsilon: Float, delta: Float)

Creates a loss descriptor with the loss function, reduction type, weight, label smoothing, and number of classes, epsilon, and delta that you specify.

### Inspecting Loss Descriptors

var lossType: MLCLossType

The loss function type.

var reductionType: MLCReductionType

The reduction operation performed by the loss function.

var weight: Float

The scale factor you apply to each element of a result.

var labelSmoothing: Float

The value for label smoothing.

var classCount: Int

The number of classes.

var epsilon: Float

The epsilon value.

var delta: Float

The delta value.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating Loss Layers with Descriptors

convenience init(descriptor: MLCLossDescriptor)

Creates a loss layer with the descriptor you specify.

Deprecated

convenience init(descriptor: MLCLossDescriptor, weights: MLCTensor)

Creates a loss layer with the descriptor and weights you specify.

Deprecated

enum MLCLossType

A loss function.

Deprecated

