

- ML Compute
- MLCEmbeddingDescriptor
-  maximumNorm Deprecated

Instance Property

# maximumNorm

A float value that, if set, causes the layer to renormalize the selected embedding vectors to have an Lp norm less than this value.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var maximumNorm: Float? { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

Renormalization occurs in the forward pass only.

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

var pNorm: Float?

The p of the Lp norm.

Deprecated

var scalesGradientByFrequency: Bool

A Boolean that indicates whether the layer scales gradients by the inverse of the frequency of words in batch before the weight update.

Deprecated

