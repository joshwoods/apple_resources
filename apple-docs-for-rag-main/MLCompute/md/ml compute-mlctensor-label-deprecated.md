

- ML Compute
- MLCTensor
-  label Deprecated

Instance Property

# label

A string that identifes this tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var label: String { get set }
```

## See Also

### Inspecting Tensors

var tensorID: Int

A number that uniquely identifies the tensor, which the framework assigns when it creates a tensor.

Deprecated

var descriptor: MLCTensorDescriptor

The configuration object you use to create a tensor.

Deprecated

var data: Data?

The tensor data.

Deprecated

var device: MLCDevice?

The device associated with this tensor.

Deprecated

var optimizerData: [MLCTensorData]

An array that contains optimizer buffers you specify when you create a tensor parameter.

Deprecated

var optimizerDeviceData: [MLCTensorOptimizerDeviceData]

An array that contains the device optimizer buffers you specify.

Deprecated

var hasValidNumerics: Bool

A Boolean that indicates whether a tensor contains NaN or INF values.

Deprecated

class MLCTensorOptimizerDeviceData

An encapsulation of the device memory associated with a tensor that an optimizer uses.

Deprecated

