

- ML Compute
-  MLCActivationLayer Deprecated

Class

# MLCActivationLayer

A layer that applies an activation function to the source tensor and produces an output.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCActivationLayer
```

## Overview

To construct an activation layer, create an activation descriptor and then pass it to the initializer.

Tip

If you don’t need to customize the behavior of the activation layer, you can save time by using Preconfigured Activation Layers instead of creating a descriptor to use with an activation layer initializer.

## Topics

### Creating Activation Layers

convenience init(descriptor: MLCActivationDescriptor)

Creates an activation layer with the descriptor you specify.

Preconfigured Activation Layers

Obtain a preconfigured activation layer with common behavior.

class MLCActivationDescriptor

A configuration object you use to create an activation layer.

### Inspecting Activation Layers

var descriptor: MLCActivationDescriptor

The configuration object you use to create an activation layer.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Activation Layers

class MLCMultiheadAttentionLayer

A multihead, scaled dot-product attention layer that attends to one or more entries in the input key-value pairs.

Deprecated

class MLCSoftmaxLayer

A layer that outputs a probability distribution as attention weights.

Deprecated

