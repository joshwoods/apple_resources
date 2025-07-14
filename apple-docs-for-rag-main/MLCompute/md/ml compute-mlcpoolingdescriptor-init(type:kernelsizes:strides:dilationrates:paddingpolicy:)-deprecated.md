

- ML Compute
- MLCPoolingDescriptor
-  init(type:kernelSizes:strides:dilationRates:paddingPolicy:) Deprecated

Initializer

# init(type:kernelSizes:strides:dilationRates:paddingPolicy:)

Creates a pooling descriptor with the pooling function type, kernel sizes, strides, dilation rates, and padding policy that you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init(
    type: MLCPoolingType,
    kernelSizes: (height: Int, width: Int),
    strides: (y: Int, x: Int) = (y: 1, x: 1),
    dilationRates: (y: Int, x: Int) = (y: 1, x: 1),
    paddingPolicy: MLCPaddingPolicy = .same
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`type`  

The pooling function type.

`kernelSizes`  

A tuple that contains the kernel sizes for y and x.

`strides`  

A tuple that contains the kernel strides for y and x.

`dilationRates`  

A tuple that contains the dilation rates for y and x.

`paddingPolicy`  

The padding policy.

