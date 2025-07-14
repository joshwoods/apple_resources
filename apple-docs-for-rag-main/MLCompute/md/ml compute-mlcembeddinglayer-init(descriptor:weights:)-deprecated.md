

- ML Compute
- MLCEmbeddingLayer
-  init(descriptor:weights:) Deprecated

Initializer

# init(descriptor:weights:)

Creates an embedding layer with the descriptor and word embedding weights tensor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    descriptor: MLCEmbeddingDescriptor,
    weights: MLCTensor
)
```

## Parameters 

`descriptor`  

An object you use to configure the embedding layer.

`weights`  

A word embedding weights tensor.

## See Also

### Creating Embedding Layers

class MLCEmbeddingDescriptor

A configuration object you use to create an embedding layer.

Deprecated

