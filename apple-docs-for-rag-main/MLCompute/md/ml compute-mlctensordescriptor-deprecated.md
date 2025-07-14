

- ML Compute
-  MLCTensorDescriptor Deprecated

Class

# MLCTensorDescriptor

A configuration object you use to create a tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCTensorDescriptor
```

## Overview

This class contains the mathematical properties of a tensor, such as data type and shape. It also includes initializers that help you create a tensor descriptor for common use cases, such as convolutional neural networks and recurrent neural networks.

## Topics

### Creating Tensor Descriptors

convenience init?(shape: [Int], dataType: MLCDataType)

Creates a tensor descriptor with the shape and data type you specify.

convenience init?(shape: [Int], sequenceLengths: [Int], sortedSequences: Bool, dataType: MLCDataType)

Creates a tensor descriptor with the shape, variable sequence lengths, sorting indicator, and data type you specify.

convenience init?(width: Int, height: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor descriptor with the width and height, number of feature channels, and batch size you specify.

convenience init?(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, dataType: MLCDataType)

Creates a tensor descriptor with the width and height, number of feature channels, batch size, and data type you specify.

convenience init?(convolutionWeightsWithInputFeatureChannelCount: Int, outputFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the number of feature channels and data type you specify.

convenience init?(convolutionWeightsWithWidth: Int, height: Int, inputFeatureChannelCount: Int, outputFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the sizing, number of feature channels, and data type you specify.

convenience init?(convolutionBiasesWithFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the number of feature channels and data type you specify.

class var maxTensorDimensions: Int

The maximum number of tensor dimensions.

### Inspecting Tensor Descriptors

var dataType: MLCDataType

The tensor data type.

var dimensionCount: Int

The number of dimensions in the tensor.

var shape: [Int]

An array that contains the size in each dimension.

var stride: [Int]

An array that contains the stride, in bytes, in each dimension.

var tensorAllocationSizeInBytes: Int

The allocation size, in bytes, for a tensor.

var sequenceLengths: [Int]?

An array that contains the variable lengths of sequences stored in the tensor.

var sortedSequences: Bool

A Boolean that indicates whether you provided the sequence lengths sorted in descending order.

var batchSizePerSequenceStep: [Int]?

The batch size for each sequence.

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

### Creating Tensors with Descriptors

convenience init(descriptor: MLCTensorDescriptor)

Creates a tensor without data, using the descriptor you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, data: MLCTensorData)

Creates a tensor with the descriptor and data you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, fillWithData: NSNumber)

Creates a tensor with the descriptor and scalar value you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the descriptor and random initializer type you specify.

Deprecated

enum MLCDataType

A tensor data type.

Deprecated

class MLCTensorData

An encapsulation of the memory that tensor data uses.

Deprecated

enum MLCRandomInitializerType

An initializer type you use to create a tensor with random data.

Deprecated

