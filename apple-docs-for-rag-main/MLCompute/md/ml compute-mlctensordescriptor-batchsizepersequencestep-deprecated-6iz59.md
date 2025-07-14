

- ML Compute
- MLCTensorDescriptor
-  batchSizePerSequenceStep Deprecated

Instance Property

# batchSizePerSequenceStep

The batch size for each sequence.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var batchSizePerSequenceStep: [Int]? { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

The framework only populates this value when sequenceLengths is valid. The length of this array is equal to the maximum sequence length in `sequenceLengths`; that is, `sequenceLengths[0]` when sortedSequences is `true`.

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

var sequenceLengths: [Int]?

An array that contains the variable lengths of sequences stored in the tensor.

Deprecated

var sortedSequences: Bool

A Boolean that indicates whether you provided the sequence lengths sorted in descending order.

Deprecated

