

- ML Compute
- MLCMultiheadAttentionLayer
-  descriptor Deprecated

Instance Property

# descriptor

The configuration object you use to create the multi-head attention layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
@NSCopying
var descriptor: MLCMultiheadAttentionDescriptor { get }
```

## See Also

### Inspecting Multi-Head Attention Layers

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

var biasesParameters: [MLCTensorParameter]?

The array of biases tensor parameters you use for optimizer updates.

Deprecated

