

- ML Compute
-  MLCPoolingDescriptor Deprecated

Class

# MLCPoolingDescriptor

A configuration object you use to create a pooling layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCPoolingDescriptor
```

## Topics

### Creating Pooling Descriptors

convenience init(type: MLCPoolingType, kernelSizes: (height: Int, width: Int), strides: (y: Int, x: Int), dilationRates: (y: Int, x: Int), paddingPolicy: MLCPaddingPolicy)

Creates a pooling descriptor with the pooling function type, kernel sizes, strides, dilation rates, and padding policy that you specify.

### Inspecting Pooling Descriptors

var poolingType: MLCPoolingType

The pooling operation type.

var kernelSizes: (height: Int, width: Int)

A tuple that contains the kernel sizes for height and width.

var strides: (y: Int, x: Int)

A tuple that contains the kernel strides for y and x.

var dilationRates: (y: Int, x: Int)

A tuple that contains the dilation rates for y and x.

var paddingPolicy: MLCPaddingPolicy

The padding policy.

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

### Creating Pooling Layers

convenience init(descriptor: MLCPoolingDescriptor)

Creates a pooling layer with the descriptor you specify.

Deprecated

enum MLCPoolingType

A pooling function type for a pooling layer.

Deprecated

