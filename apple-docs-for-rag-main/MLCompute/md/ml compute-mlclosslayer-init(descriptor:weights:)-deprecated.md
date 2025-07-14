

- ML Compute
- MLCLossLayer
-  init(descriptor:weights:) Deprecated

Initializer

# init(descriptor:weights:)

Creates a loss layer with the descriptor and weights you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    descriptor lossDescriptor: MLCLossDescriptor,
    weights: MLCTensor
)
```

## Parameters 

`lossDescriptor`  

An object you use to configure the loss layer.

`weights`  

The loss label weights tensor.

## See Also

### Creating Loss Layers with Descriptors

convenience init(descriptor: MLCLossDescriptor)

Creates a loss layer with the descriptor you specify.

Deprecated

class MLCLossDescriptor

A configuration object you use to create a loss layer.

Deprecated

enum MLCLossType

A loss function.

Deprecated

