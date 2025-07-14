

- ML Compute
- MLCLSTMLayer
-  init(descriptor:inputWeights:hiddenWeights:peepholeWeights:biases:) Deprecated

Initializer

# init(descriptor:inputWeights:hiddenWeights:peepholeWeights:biases:)

Creates an LSTM layer with the descriptor, weights, and biases you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    descriptor: MLCLSTMDescriptor,
    inputWeights: [MLCTensor],
    hiddenWeights: [MLCTensor],
    peepholeWeights: [MLCTensor]?,
    biases: [MLCTensor]?
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

## See Also

### Creating LSTM Layers

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, input and hidden weights, and biases you specify.

Deprecated

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?, gateActivations: [MLCActivationDescriptor], outputResultActivation: MLCActivationDescriptor)

Creates an LSTM layer using the descriptor, weights, biases, gate activations, and output result activation that you specify.

Deprecated

class MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

Deprecated

enum MLCLSTMResultMode

Constants that describe the result of an LSTM layer.

Deprecated

