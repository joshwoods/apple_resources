

- ML Compute
- MLCTransposeLayer
-  dimensions Deprecated

Instance Property

# dimensions

An array that contains an input axis source for each output axis, which represents the ordering of dimensions.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var dimensions: [Int] { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

Permutes the dimensions according to `dimensions`. The returned tensor’s dimension `i` corresponds to `dimensions[i]`.

