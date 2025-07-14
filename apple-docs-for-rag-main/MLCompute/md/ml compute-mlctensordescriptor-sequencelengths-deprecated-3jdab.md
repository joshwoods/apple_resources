

- ML Compute
- MLCTensorDescriptor
-  sequenceLengths Deprecated

Instance Property

# sequenceLengths

An array that contains the variable lengths of sequences stored in the tensor.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var sequenceLengths: [Int]? { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## See Also

### Inspecting Tensor Descriptors

var dataType: MLCDataType

The tensor data type.

Deprecated

var dimensionCount: Int

The number of dimensions in the tensor.

Deprecated

var shape: [Int]

An array that contains the size in each dimension.

Deprecated

var stride: [Int]

An array that contains the stride, in bytes, in each dimension.

Deprecated

var tensorAllocationSizeInBytes: Int

The allocation size, in bytes, for a tensor.

Deprecated

var sortedSequences: Bool

A Boolean that indicates whether you provided the sequence lengths sorted in descending order.

Deprecated

var batchSizePerSequenceStep: [Int]?

The batch size for each sequence.

Deprecated

