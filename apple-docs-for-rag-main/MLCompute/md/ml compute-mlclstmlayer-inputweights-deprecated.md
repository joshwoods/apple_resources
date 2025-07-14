

- ML Compute
- MLCLSTMLayer
-  inputWeights Deprecated

Instance Property

# inputWeights

The array of tensors that describe the input weights you use for the input, hidden, cell, and output gates.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var inputWeights: [MLCTensor] { get }
```

## See Also

### Inspecting LSTM Layers

var descriptor: MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

Deprecated

var gateActivations: [MLCActivationDescriptor]

The array of gate activations you use for input, hidden, cell, and output gates.

Deprecated

var outputResultActivation: MLCActivationDescriptor

The output activation descriptor.

Deprecated

var hiddenWeights: [MLCTensor]

The array of tensors that describe the hidden weights you use for the input, hidden, cell, and output gates.

Deprecated

var peepholeWeights: [MLCTensor]?

The array of tensors that describe the peephole weights you use for the input, hidden, cell, and output gates.

Deprecated

var biases: [MLCTensor]?

The array of tensors that describe the bias terms you use for the input, hidden, cell, and output gates.

Deprecated

var inputWeightsParameters: [MLCTensorParameter]

The input weights tensor parameters you use for optimizer updates.

Deprecated

var hiddenWeightsParameters: [MLCTensorParameter]

The hidden weights tensor parameters you use for optimizer updates.

Deprecated

var peepholeWeightsParameters: [MLCTensorParameter]?

The peephole weights tensor parameters you use for optimizer updates.

Deprecated

var biasesParameters: [MLCTensorParameter]?

The biases tensor parameters you use for optimizer updates.

Deprecated

