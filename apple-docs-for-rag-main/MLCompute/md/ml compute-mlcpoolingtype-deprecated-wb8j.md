

- ML Compute
-  MLCPoolingType Deprecated

Enumeration

# MLCPoolingType

A pooling function type for a pooling layer.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
enum MLCPoolingType
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Topics

### Enumeration Cases

case max

case average(countIncludesPadding: Bool)

case l2Norm

var debugDescription: String

A textual description of the pooling type, suitable for debugging.

## See Also

### Creating Pooling Layers

convenience init(descriptor: MLCPoolingDescriptor)

Creates a pooling layer with the descriptor you specify.

Deprecated

class MLCPoolingDescriptor

A configuration object you use to create a pooling layer.

Deprecated

