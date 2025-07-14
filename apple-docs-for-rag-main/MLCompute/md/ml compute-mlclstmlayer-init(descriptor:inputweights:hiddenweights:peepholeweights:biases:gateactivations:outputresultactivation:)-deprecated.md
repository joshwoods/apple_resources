

- ML Compute
- MLCLSTMLayer
-  init(descriptor:inputWeights:hiddenWeights:peepholeWeights:biases:gateActivations:outputResultActivation:) Deprecated

Initializer

# init(descriptor:inputWeights:hiddenWeights:peepholeWeights:biases:gateActivations:outputResultActivation:)

Creates an LSTM layer using the descriptor, weights, biases, gate activations, and output result activation that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    descriptor: MLCLSTMDescriptor,
    inputWeights: [MLCTensor],
    hiddenWeights: [MLCTensor],
    peepholeWeights: [MLCTensor]?,
    biases: [MLCTensor]?,
    gateActivations: [MLCActivationDescriptor],
    outputResultActivation: MLCActivationDescriptor
)
```

## Parameters 

`descriptor`  

An object you use to configure the LSTM layer.

`inputWeights`  

An array that contains tensors that describe the input weights.

`hiddenWeights`  

An array that contains tensors that describe the hidden weights.

`peepholeWeights`  

An array that contains tensors that describe the peephole weights.

`biases`  

An array that contains tensors that describe the bias terms.

`gateActivations`  

An array that contains 4 neuron descriptors for the input, hidden, cell, and output gate activations.

`outputResultActivation`  

The neuron descriptor you use for the activation function applied to output result. The default value is tanh.

## See Also

### Creating LSTM Layers

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, input and hidden weights, and biases you specify.

Deprecated

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, weights, and biases you specify.

Deprecated

class MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

Deprecated

enum MLCLSTMResultMode

Constants that describe the result of an LSTM layer.

Deprecated

