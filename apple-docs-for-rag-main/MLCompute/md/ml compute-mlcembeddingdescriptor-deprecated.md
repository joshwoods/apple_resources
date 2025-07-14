

- ML Compute
-  MLCEmbeddingDescriptor Deprecated

Class

# MLCEmbeddingDescriptor

A configuration object you use to create an embedding layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCEmbeddingDescriptor
```

## Topics

### Creating Embedding Descriptors

convenience init?(embeddingCount: Int, embeddingDimension: Int)

Creates an embedding descriptor with the size of the dictionary and dimension of embedding vectors you specify.

convenience init?(embeddingCount: Int, embeddingDimension: Int, paddingIndex: Int?, maximumNorm: Float?, pNorm: Float?, scalesGradientByFrequency: Bool)

Creates an embedding descriptor with the size and dimension of embedding vectors, padding index, and norm and scaling options that you specify.

### Inspecting Embedding Descriptors

var embeddingCount: Int

The size of the dictionary.

var embeddingDimension: Int

The dimension of embedding vectors.

var paddingIndex: Int?

An unsigned integer value that, if set, causes the layer to initialize the embedding vector at that index to zero.

var maximumNorm: Float?

A float value that, if set, causes the layer to renormalize the selected embedding vectors to have an Lp norm less than this value.

var pNorm: Float?

The p of the Lp norm.

var scalesGradientByFrequency: Bool

A Boolean that indicates whether the layer scales gradients by the inverse of the frequency of words in batch before the weight update.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating Embedding Layers

convenience init(descriptor: MLCEmbeddingDescriptor, weights: MLCTensor)

Creates an embedding layer with the descriptor and word embedding weights tensor you specify.

Deprecated

