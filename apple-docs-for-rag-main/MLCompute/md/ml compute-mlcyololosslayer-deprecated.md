

- ML Compute
-  MLCYOLOLossLayer Deprecated

Class

# MLCYOLOLossLayer

A layer that estimates loss for the YOLO algorithm.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCYOLOLossLayer
```

## Topics

### Creating YOLO Loss Layers

convenience init(descriptor: MLCYOLOLossDescriptor)

Creates a YOLO loss layer with the descriptor you specify.

class MLCYOLOLossDescriptor

The configuration object you use to create the YOLO loss layer.

### Inspecting YOLO Loss Layers

var yoloLossDescriptor: MLCYOLOLossDescriptor

The configuration object you use to create the YOLO loss layer.

## Relationships

### Inherits From

- MLCLossLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Loss Layers

class MLCLossLayer

A layer that estimates the inaccuracies of the model to reduce the loss on the next evaluation.

Deprecated

