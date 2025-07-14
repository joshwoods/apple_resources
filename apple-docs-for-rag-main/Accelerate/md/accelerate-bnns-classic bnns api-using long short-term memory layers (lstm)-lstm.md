

- Accelerate
- BNNS
- Classic BNNS API
-  Using Long Short-Term Memory Layers (LSTM) 

Article

# Using Long Short-Term Memory Layers (LSTM)

Add long short-term memory (LSTM) layers to recurrent neural networks to avoid long-term dependency problems.

## Overview

An LSTM layer consists of four gates that manipulate cell-state data:

Forget gate  
Controls whether to erase data from the cell-state.

Input gate  
Controls whether to write data to the cell-state.

Candidate gate  
Controls what data to write to the cell-state.

Output gate  
Controls what data to pass as the output hidden state.

The following figure illustrates the components of an LSTM layer. The inputs are the cell-state (c), the hidden state (h), and the input data (x). The outputs are the updated cell-state (c) and hidden state (h):

Note that the default activation function for the forget, input, and output gates is sigmoid; the default activation function for the candidate gate is tanh.

BNNS provides direct apply functions for forward and backward LSTM passes, that is, you don’t need to create an explicit LSTM layer. Rather, you create descriptors of the input, output, and gates to create a parameters structure, and pass the parameters structure to the apply function.

The input and out descriptors require n-dimensional array descriptors for the data, hidden state, and cell-state:

```
let inputDescriptor = BNNSLSTMDataDescriptor(data_desc: inputDataDescriptor,
                                             hidden_desc: inputHiddenDescriptor,
                                             cell_state_desc: inputCellStateDescriptor)

let outputDescriptor = BNNSLSTMDataDescriptor(data_desc: outputDataDescriptor,
                                              hidden_desc: outputHiddenDescriptor,
                                              cell_state_desc: outputCellStateDescriptor)
```

Define each gate by specifying input, hidden, and cell-state weights, and bias:

```
let forgetGate = BNNSLSTMGateDescriptor(iw_desc: (forgetGateInputWeightsDescriptor,
                                                  forgetGateInputWeightsDescriptor),
                                        hw_desc: forgetGateHiddenWeightsDescriptor,
                                        cw_desc: forgetGateCellStateWeightsDescriptor,
                                        b_desc: forgetGateBiasDescriptor,
                                        activation: BNNSActivation(function: .sigmoid))

let inputGate = BNNSLSTMGateDescriptor(iw_desc: (inputGateInputWeightsDescriptor,
                                                 inputGateInputWeightsDescriptor),
                                       hw_desc: inputGateHiddenWeightsDescriptor,
                                       cw_desc: inputGateCellStateWeightsDescriptor,
                                       b_desc: inputGateBiasDescriptor,
                                       activation: BNNSActivation(function: .sigmoid))

let candidateGate = BNNSLSTMGateDescriptor(iw_desc: (candidateGateInputWeightsDescriptor,
                                                     candidateGateInputWeightsDescriptor),
                                           hw_desc: candidateGateHiddenWeightsDescriptor,
                                           cw_desc: candidateGateCellStateWeightsDescriptor,
                                           b_desc: candidateGateBiasDescriptor,
                                           activation: BNNSActivation(function: .tanh))

let outputGate = BNNSLSTMGateDescriptor(iw_desc: (outputGateInputWeightsDescriptor,
                                                  outputGateInputWeightsDescriptor),
                                        hw_desc: outputGateHiddenWeightsDescriptor,
                                        cw_desc: outputGateCellStateWeightsDescriptor,
                                        b_desc: outputGateBiasDescriptor,
                                        activation: BNNSActivation(function: .sigmoid))
```

The following code shows how each gate computes its output:

```
 for (size_t o = 0; o 

Give the descriptors for the input, output, and gates, you’re ready to create the parameters structure:

```
var layerParams = BNNSLayerParametersLSTM(input_size:  ... ,
                                          hidden_size:  ... ,
                                          batch_size: ... ,
                                          num_layers: ... ,
                                          seq_len: ... ,
                                          dropout: ... ,
                                          lstm_flags: BNNSLayerFlagsLSTMDefaultActivations.rawValue,
                                          sequence_descriptor: BNNSNDArrayDescriptor(),
                                          input_descriptor: inputDescriptor,
                                          output_descriptor: outputDescriptor,
                                          input_gate: inputGate,
                                          forget_gate: forgetGate,
                                          candidate_gate: candidateGate,
                                          output_gate: outputGate,
                                          hidden_activation: BNNSActivation(function: .identity))
```

LSTM provides the option to define a training cache that stores intermediate results to accelerate backward computation. Use BNNSComputeLSTMTrainingCacheCapacity(_:) to compute the size, in bytes, of the training cache:

```
let trainingCacheBufferBytes = BNNSComputeLSTMTrainingCacheCapacity(&layerParams)

let trainingCache = UnsafeMutableRawPointer.allocate(byteCount: trainingCacheBufferBytes,
                                                     alignment: 1)
defer {
    trainingCache.deallocate()
}
```

Finally, call BNNSDirectApplyLSTMBatchTrainingCaching(_:_:_:_:) to apply the LSTM layer:

```
BNNSDirectApplyLSTMBatchTrainingCaching(&layerParams,
                                        nil,
                                        trainingCache,
                                        trainingCacheBufferBytes)
```

## See Also

### Recurrent layers

struct BNNSLSTMDataDescriptor

A structure that contains the input-output, hidden, and cell state n-dimensional array descriptors for a long short-term memory (LSTM) layer.

Deprecated

struct BNNSLSTMGateDescriptor

A structure that describes a long short-term memory (LSTM) gate layer.

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

