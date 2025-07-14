

- Metal Performance Shaders Graph
-  MPSGraphPooling2DOpDescriptor 

Class

# MPSGraphPooling2DOpDescriptor

The class that defines the parameters for a 2D pooling operation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphPooling2DOpDescriptor
```

## Overview

Use this descriptor with the following methods:

- maxPooling2D(withSourceTensor:descriptor:name:)

- maxPooling2DReturnIndices(_:descriptor:name:)

- maxPooling2DGradient(withGradientTensor:sourceTensor:descriptor:name:)

- maxPooling2DGradient(withGradientTensor:indicesTensor:outputShape:descriptor:name:)

- maxPooling2DGradient(withGradientTensor:indicesTensor:outputShapeTensor:descriptor:name:)

- avgPooling2D(withSourceTensor:descriptor:name:)

- avgPooling2DGradient(withGradientTensor:sourceTensor:descriptor:name:)

## Topics

### Initializers

convenience init?(kernelWidth: Int, kernelHeight: Int, strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, paddingLeft: Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout)

Creates a 2D pooling descriptor with given values.

convenience init?(kernelWidth: Int, kernelHeight: Int, strideInX: Int, strideInY: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout)

Creates a 2D pooling descriptor with given values.

### Instance Properties

var ceilMode: Bool

Affects how the graph computes the output size.

var dataLayout: MPSGraphTensorNamedDataLayout

Defines the data layout of the input data in the forward pass. See: MPSGraphTensorNamedDataLayout.

var dilationRateInX: Int

Defines the dilation rate for the width dimension.

var dilationRateInY: Int

Defines the dilation rate for the height dimension.

var includeZeroPadToAverage: Bool

Defines a mode for average pooling, where samples outside the input tensor count as zeroes in the average computation.

var kernelHeight: Int

Defines the pooling window size for the height dimension.

var kernelWidth: Int

Defines the pooling window size for the width dimension.

var paddingBottom: Int

Defines the explicit padding value for the height dimension to add after the data.

var paddingLeft: Int

Defines the explicit padding value for the width dimension to add before the data.

var paddingRight: Int

Defines the explicit padding value for the width dimension to add after the data.

var paddingStyle: MPSGraphPaddingStyle

Defines what kind of padding graph applies to the operation.

var paddingTop: Int

Defines the explicit padding value for the height dimension to add before the data.

var returnIndicesDataType: MPSDataType

Defines the data type for returned indices. Use this in conjunction with maxPooling2DReturnIndices(_:descriptor:name:) API. Currently MPSGraph supports the following datatypes: `MPSDataTypeInt32`. Default value: `MPSDataTypeInt32`.

var returnIndicesMode: MPSGraphPoolingReturnIndicesMode

Defines the mode for returned indices of maximum values within each pooling window. Use this in conjunction with maxPooling2DReturnIndices(_:descriptor:name:) API. If `returnIndicesMode = MPSGraphPoolingReturnIndicesNone` then only the first result MPSGraph returns from maxPooling2DReturnIndices(_:descriptor:name:) will be valid and using the second result will assert. Default value: `MPSGraphPoolingReturnIndicesNone`.

var strideInX: Int

Defines the stride for the width dimension.

var strideInY: Int

Defines the stride for the height dimension.

### Instance Methods

func setExplicitPaddingWithPaddingLeft(Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int)

Sets the explicit padding values and sets padding style to explicit.

## Relationships

### Inherits From

- MPSGraphObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Classes

class MPSGraph

The optimized representation of a compute graph of operations and tensors.

class MPSGraphCompilationDescriptor

A class that consists of all the levers for compiling graphs.

class MPSGraphConvolution2DOpDescriptor

A class that describes the properties of a 2D-convolution operator.

class MPSGraphConvolution3DOpDescriptor

A class that describes the properties of a 3D-convolution operator.

class MPSGraphCreateSparseOpDescriptor

A class that describes the properties of a create sparse operation.

class MPSGraphDepthwiseConvolution2DOpDescriptor

A class that defines the parameters for a 2D-depthwise convolution operation.

class MPSGraphDepthwiseConvolution3DOpDescriptor

The class that defines the parameters for a 3D-depthwise convolution operation.

class MPSGraphDevice

A class that describes the compute device.

class MPSGraphExecutable

The compiled representation of a compute graph executable.

class MPSGraphExecutableExecutionDescriptor

A class that consists of all the levers to synchronize and schedule executable execution.

class MPSGraphExecutableSerializationDescriptor

A class that consists of all the levers to serialize an executable.

class MPSGraphExecutionDescriptor

A class that consists of all the levers to synchronize and schedule graph execution.

class MPSGraphFFTDescriptor

The class that defines the parameters for a fast Fourier transform (FFT) operation.

class MPSGraphGRUDescriptor

The class that defines the parameters for a gated recurrent unit (GRU) operation.

class MPSGraphImToColOpDescriptor

The class that defines the parameters for an image to column or column to image operation.

