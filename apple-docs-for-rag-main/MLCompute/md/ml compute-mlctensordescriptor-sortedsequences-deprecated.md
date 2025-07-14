

- ML Compute
- MLCTensorDescriptor
-  sortedSequences Deprecated

Instance Property

# sortedSequences

A Boolean that indicates whether you provided the sequence lengths sorted in descending order.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var sortedSequences: Bool { get }
```

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

var batchSizePerSequenceStep: [Int]?

The batch size for each sequence.

Deprecated

