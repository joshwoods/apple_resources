

- ML Compute
- MLCMultiheadAttentionLayer
-  biasesParameters Deprecated

Instance Property

# biasesParameters

The array of biases tensor parameters you use for optimizer updates.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var biasesParameters: [MLCTensorParameter]? { get }
```

## See Also

### Inspecting Multi-Head Attention Layers

var descriptor: MLCMultiheadAttentionDescriptor

The configuration object you use to create the multi-head attention layer.

Deprecated

var weights: [MLCTensor]

The array of weights you use for query, key, value, and output projections.

Deprecated

var biases: [MLCTensor]?

The array of biases you use for query, key, value, and output projections.

Deprecated

var attentionBiases: [MLCTensor]?

The array of attention biases you use for key and value.

Deprecated

var weightsParameters: [MLCTensorParameter]

The array of weights tensor parameters you use for optimizer updates.

Deprecated

