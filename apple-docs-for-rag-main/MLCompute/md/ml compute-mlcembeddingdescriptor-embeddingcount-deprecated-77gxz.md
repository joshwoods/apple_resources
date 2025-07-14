

- ML Compute
- MLCEmbeddingDescriptor
-  embeddingCount Deprecated

Instance Property

# embeddingCount

The size of the dictionary.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var embeddingCount: Int { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## See Also

### Inspecting Embedding Descriptors

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

var scalesGradientByFrequency: Bool

A Boolean that indicates whether the layer scales gradients by the inverse of the frequency of words in batch before the weight update.

Deprecated

