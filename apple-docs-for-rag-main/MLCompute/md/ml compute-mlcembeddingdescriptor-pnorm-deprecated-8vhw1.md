

- ML Compute
- MLCEmbeddingDescriptor
-  pNorm Deprecated

Instance Property

# pNorm

The p of the Lp norm.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var pNorm: Float? { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

You can set this value to infinity.

## See Also

### Inspecting Embedding Descriptors

var embeddingCount: Int

The size of the dictionary.

Deprecated

var embeddingDimension: Int

The dimension of embedding vectors.

Deprecated

var paddingIndex: Int?

An unsigned integer value that, if set, causes the layer to initialize the embedding vector at that index to zero.

Deprecated

var maximumNorm: Float?

A float value that, if set, causes the layer to renormalize the selected embedding vectors to have an Lp norm less than this value.

Deprecated

var scalesGradientByFrequency: Bool

A Boolean that indicates whether the layer scales gradients by the inverse of the frequency of words in batch before the weight update.

Deprecated

