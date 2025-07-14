

- Accelerate
-  BNNSLSTMGateDescriptor Deprecated

Structure

# BNNSLSTMGateDescriptor

A structure that describes a long short-term memory (LSTM) gate layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLSTMGateDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(iw_desc: (BNNSNDArrayDescriptor, BNNSNDArrayDescriptor), hw_desc: BNNSNDArrayDescriptor, cw_desc: BNNSNDArrayDescriptor, b_desc: BNNSNDArrayDescriptor, activation: BNNSActivation)

Returns a new long short-term memory (LSTM) gate descriptor structure from the specified parameters.

init()

Returns a new long short-term memory (LSTM) gate descriptor structure.

### Instance Properties

var iw_desc: (BNNSNDArrayDescriptor, BNNSNDArrayDescriptor)

The descriptor of the input weights.

var hw_desc: BNNSNDArrayDescriptor

The descriptor of the hidden weights.

var cw_desc: BNNSNDArrayDescriptor

The descriptor of the cell weights.

var b_desc: BNNSNDArrayDescriptor

The descriptor of the bias.

var activation: BNNSActivation

The activation function that the layer applies to the output.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Recurrent layers

Using Long Short-Term Memory Layers (LSTM)

Add long short-term memory (LSTM) layers to recurrent neural networks to avoid long-term dependency problems.

struct BNNSLSTMDataDescriptor

A structure that contains the input-output, hidden, and cell state n-dimensional array descriptors for a long short-term memory (LSTM) layer.

Deprecated

struct BNNSLayerFlags

Options that control the behavior of a long short-term memory (LSTM) layer.

struct BNNSLayerParametersLSTM

A structure that contains the parameters of a long short-term memory (LSTM) layer.

Deprecated

func BNNSComputeLSTMTrainingCacheCapacity(UnsafePointer&lt;BNNSLayerParametersLSTM>) -> Int

Returns the minimum bytes capacity of the training cache buffer a long short-term memory (LSTM) layer uses when it’s applied.

Deprecated

func BNNSDirectApplyLSTMBatchTrainingCaching(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeMutableRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) layer directly to an input.

Deprecated

func BNNSDirectApplyLSTMBatchBackward(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) filter backward to generate gradients.

Deprecated

