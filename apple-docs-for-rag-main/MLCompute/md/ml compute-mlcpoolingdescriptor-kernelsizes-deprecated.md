

- ML Compute
- MLCPoolingDescriptor
-  kernelSizes Deprecated

Instance Property

# kernelSizes

A tuple that contains the kernel sizes for height and width.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var kernelSizes: (height: Int, width: Int) { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## See Also

### Inspecting Pooling Descriptors

var poolingType: MLCPoolingType

The pooling operation type.

Deprecated

var strides: (y: Int, x: Int)

A tuple that contains the kernel strides for y and x.

Deprecated

var dilationRates: (y: Int, x: Int)

A tuple that contains the dilation rates for y and x.

Deprecated

var paddingPolicy: MLCPaddingPolicy

The padding policy.

Deprecated

