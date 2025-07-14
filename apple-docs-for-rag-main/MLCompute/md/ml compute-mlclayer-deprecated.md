

- ML Compute
-  MLCLayer Deprecated

Class

# MLCLayer

The base class for all framework layers.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLayer
```

## Overview

This class defines a polymorphic interface for `MLCLayer` subclasses. There are subclasses for each supported neural network layer type. Use the appropriate subclass initializer to create a layer object.

## Topics

### Inspecting a Layer

var layerID: Int

A unique number that identifies each layer.

var label: String

A string that helps identify this layer.

var isDebuggingEnabled: Bool

A Boolean that indicates whether you choose to debug the layer when executing a graph that includes it.

var deviceType: MLCDeviceType

A device type that indicates where the system executes the layer.

class func supportsDataType(MLCDataType, on: MLCDevice) -> Bool

Returns a Boolean that indicates whether instances of this layer accept source tensors for the data type and device that you specify.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MLCActivationLayer
- MLCArithmeticLayer
- MLCBatchNormalizationLayer
- MLCComparisonLayer
- MLCConcatenationLayer
- MLCConvolutionLayer
- MLCDropoutLayer
- MLCEmbeddingLayer
- MLCFullyConnectedLayer
- MLCGatherLayer
- MLCGramMatrixLayer
- MLCGroupNormalizationLayer
- MLCInstanceNormalizationLayer
- MLCLSTMLayer
- MLCLayerNormalizationLayer
- MLCLossLayer
- MLCMatMulLayer
- MLCMultiheadAttentionLayer
- MLCPaddingLayer
- MLCPoolingLayer
- MLCReductionLayer
- MLCReshapeLayer
- MLCScatterLayer
- MLCSelectionLayer
- MLCSliceLayer
- MLCSoftmaxLayer
- MLCSplitLayer
- MLCTransposeLayer
- MLCUpsampleLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

