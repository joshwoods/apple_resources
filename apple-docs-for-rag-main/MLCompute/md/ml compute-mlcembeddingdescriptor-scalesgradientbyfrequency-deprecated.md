

- ML Compute
- MLCEmbeddingDescriptor
-  scalesGradientByFrequency Deprecated

Instance Property

# scalesGradientByFrequency

A Boolean that indicates whether the layer scales gradients by the inverse of the frequency of words in batch before the weight update.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var scalesGradientByFrequency: Bool { get }
```

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

var pNorm: Float?

The p of the Lp norm.

Deprecated

