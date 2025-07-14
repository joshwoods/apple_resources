

- Accelerate
-  BNNSLayerParametersLSTM Deprecated

Structure

# BNNSLayerParametersLSTM

A structure that contains the parameters of a long short-term memory (LSTM) layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersLSTM
```

Deprecated

Use BNNSGraph\* APIs

## Overview

Use a BNNSLayerParametersLSTM structure to define the parameters of a long short-term memory (LSTM) operation.

## Topics

### Initializers

init(input_size: Int, hidden_size: Int, batch_size: Int, num_layers: Int, seq_len: Int, dropout: Float, lstm_flags: UInt32, sequence_descriptor: BNNSNDArrayDescriptor, input_descriptor: BNNSLSTMDataDescriptor, output_descriptor: BNNSLSTMDataDescriptor, input_gate: BNNSLSTMGateDescriptor, forget_gate: BNNSLSTMGateDescriptor, candidate_gate: BNNSLSTMGateDescriptor, output_gate: BNNSLSTMGateDescriptor, hidden_activation: BNNSActivation)

Returns a new long short-term memory (LSTM) parameters structure from the specified parameters.

init()

Returns a new long short-term memory (LSTM) parameters structure.

### Instance Properties

var input_size: Int

The number of elements in the input.

var hidden_size: Int

The number of elements in the hidden state.

var batch_size: Int

The number of input and output samples.

var num_layers: Int

The number of stacked long short-term memory (LSTM) layers.

var seq_len: Int

The size of the sequential input.

var dropout: Float

The dropout ratio to apply between long short-term memory (LSTM) layers.

var lstm_flags: UInt32

Flags that control the behavior of a long short-term memory (LSTM) layer.

var sequence_descriptor: BNNSNDArrayDescriptor

A 1D array of unsigned-integer elements that determines the batch size for each step.

var input_descriptor: BNNSLSTMDataDescriptor

Descriptors of the input, hidden input, and cell-state input data.

var output_descriptor: BNNSLSTMDataDescriptor

Descriptors of the output, hidden output, and cell-state output data.

var input_gate: BNNSLSTMGateDescriptor

The descriptor of the input gate, which uses default sigmoid activation.

var forget_gate: BNNSLSTMGateDescriptor

The descriptor of the forget gate, which uses default sigmoid activation.

var candidate_gate: BNNSLSTMGateDescriptor

The descriptor of the candidate gate, which uses default tanh activation.

var output_gate: BNNSLSTMGateDescriptor

The descriptor of the output gate, which uses default sigmoid activation.

var hidden_activation: BNNSActivation

Hidden activation function, which uses default tanh activation.

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

struct BNNSLSTMGateDescriptor

A structure that describes a long short-term memory (LSTM) gate layer.

Deprecated

struct BNNSLayerFlags

Options that control the behavior of a long short-term memory (LSTM) layer.

func BNNSComputeLSTMTrainingCacheCapacity(UnsafePointer&lt;BNNSLayerParametersLSTM>) -> Int

Returns the minimum bytes capacity of the training cache buffer a long short-term memory (LSTM) layer uses when it’s applied.

Deprecated

func BNNSDirectApplyLSTMBatchTrainingCaching(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeMutableRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) layer directly to an input.

Deprecated

func BNNSDirectApplyLSTMBatchBackward(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) filter backward to generate gradients.

Deprecated

