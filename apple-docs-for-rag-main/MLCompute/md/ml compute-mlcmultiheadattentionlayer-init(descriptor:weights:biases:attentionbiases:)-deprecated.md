

- ML Compute
- MLCMultiheadAttentionLayer
-  init(descriptor:weights:biases:attentionBiases:) Deprecated

Initializer

# init(descriptor:weights:biases:attentionBiases:)

Creates a multi-head attention layer with the descriptor, weights, and biases you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    descriptor: MLCMultiheadAttentionDescriptor,
    weights: [MLCTensor],
    biases: [MLCTensor]?,
    attentionBiases: [MLCTensor]?
)
```

## Parameters 

`descriptor`  

An object you use to configure the multi-head attention layer.

`weights`  

An array that contains the weights that correspond to query, key, value, and output projections for all heads.

`biases`  

An array that contains the biases that correspond to query, key, value, and output projections for all heads.

`attentionBiases`  

An array that contains the biases you add to the key and value, respectively.

## See Also

### Creating Multi-Head Attention Layers

class MLCMultiheadAttentionDescriptor

A configuration object you use to create a multi-head attention layer.

Deprecated

