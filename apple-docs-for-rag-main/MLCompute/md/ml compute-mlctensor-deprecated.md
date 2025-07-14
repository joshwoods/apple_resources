

- ML Compute
-  MLCTensor Deprecated

Class

# MLCTensor

The data object you use throughout the framework.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCTensor
```

## Overview

Create a tensor with or without data. For example, create a tensor with data for weights used by convolution or mean, variance, beta, and gamma parameters with batch normalization. Create a tensor without data to use as an input tensor when you build a graph.

## Topics

### Creating Tensors with Descriptors

convenience init(descriptor: MLCTensorDescriptor)

Creates a tensor without data, using the descriptor you specify.

convenience init(descriptor: MLCTensorDescriptor, data: MLCTensorData)

Creates a tensor with the descriptor and data you specify.

convenience init(descriptor: MLCTensorDescriptor, fillWithData: NSNumber)

Creates a tensor with the descriptor and scalar value you specify.

convenience init(descriptor: MLCTensorDescriptor, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the descriptor and random initializer type you specify.

class MLCTensorDescriptor

A configuration object you use to create a tensor.

enum MLCDataType

A tensor data type.

class MLCTensorData

An encapsulation of the memory that tensor data uses.

enum MLCRandomInitializerType

An initializer type you use to create a tensor with random data.

### Creating Tensors by Specifying Shape

convenience init(shape: [Int])

Creates a tensor without data, with the shape you specify.

convenience init(shape: [Int], dataType: MLCDataType)

Creates a tensor without data, with the shape and data type you specify.

convenience init(shape: [Int], data: MLCTensorData, dataType: MLCDataType)

Creates a tensor with the shape, data, and data type you specify.

convenience init(shape: [Int], fillWithData: NSNumber, dataType: MLCDataType)

Creates a tensor with the shape, scalar value, and data type you specify.

convenience init(shape: [Int], randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the shape and random initializer type you specify.

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor without data, with the sizes and number of feature channels you specify.

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData)

Creates a tensor with the sizes, number of feature channels, and data you specify.

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData, dataType: MLCDataType)

Creates a tensor with the sizes, number of feature channels, data, and data type you specify.

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, fillWithData: Float, dataType: MLCDataType)

Creates a tensor with the sizes and number of feature channels, and filled with the data and type you specify.

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sizes, number of feature channels, and random data using the random initializer type you specify.

### Creating Tensors by Specifying Sequence Lengths

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor without data, with the sequence length, number of feature channels, and batch size you specify.

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData?)

Creates a tensor with the sequence length, number of feature channels, batch size, and data you specify.

convenience init?(sequenceLengths: [Int], sortedSequences: Bool, featureChannelCount: Int, batchSize: Int, data: MLCTensorData?)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and data you specify.

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence length, number of feature channels, batch size, and random initializer type you specify.

convenience init?(sequenceLengths: [Int], sortedSequences: Bool, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and random initializer type you specify.

### Inspecting Tensors

var tensorID: Int

A number that uniquely identifies the tensor, which the framework assigns when it creates a tensor.

var descriptor: MLCTensorDescriptor

The configuration object you use to create a tensor.

var data: Data?

The tensor data.

var label: String

A string that identifes this tensor.

var device: MLCDevice?

The device associated with this tensor.

var optimizerData: [MLCTensorData]

An array that contains optimizer buffers you specify when you create a tensor parameter.

var optimizerDeviceData: [MLCTensorOptimizerDeviceData]

An array that contains the device optimizer buffers you specify.

var hasValidNumerics: Bool

A Boolean that indicates whether a tensor contains NaN or INF values.

class MLCTensorOptimizerDeviceData

An encapsulation of the device memory associated with a tensor that an optimizer uses.

### Converting Tensors

func quantized(to: MLCDataType, scale: Float, bias: Int) -> MLCTensor?

Converts a 32-bit floating-point tensor with the scale and bias you specify.

func quantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a 32-bit floating-point tensor with the scale and bias you specify.

func dequantized(to: MLCDataType, scale: MLCTensor, zeroPoint: MLCTensor) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

func dequantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

### Managing Tensor Data

func synchronizeData() -> Bool

Synchronizes the data in host memory.

func synchronizeOptimizerData() -> Bool

Synchronizes the optimizer data in host memory.

func copyDataFromDeviceMemory(toBytes: UnsafeMutableRawPointer, length: Int, synchronizeWithDevice: Bool) -> Bool

Copies tensor data from device memory to user-specified memory.

func bindAndWriteData(MLCTensorData, to: MLCDevice) -> Bool

Associates the given data to the tensor, and if the device is a GPU, also copies the data to the device memory.

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?) -> Bool

Associates the optimizer and device data buffers you specify to the tensor.

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

### Components

class MLCPlatform

A utility class for setting global properties in the framework.

Deprecated

Layers

Create and inspect layers that encapsulate operations and configuration details to receive, process, and output tensors.

Training and Validation

Create, train, and validate a graph to produce acceptable prediction results.

