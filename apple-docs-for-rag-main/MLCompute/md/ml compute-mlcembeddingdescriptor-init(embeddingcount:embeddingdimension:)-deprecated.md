

- ML Compute
- MLCEmbeddingDescriptor
-  init(embeddingCount:embeddingDimension:) Deprecated

Initializer

# init(embeddingCount:embeddingDimension:)

Creates an embedding descriptor with the size of the dictionary and dimension of embedding vectors you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    embeddingCount: Int,
    embeddingDimension: Int
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`embeddingCount`  

The size of the dictionary.

`embeddingDimension`  

The dimension of embedding vectors.

## See Also

### Creating Embedding Descriptors

convenience init?(embeddingCount: Int, embeddingDimension: Int, paddingIndex: Int?, maximumNorm: Float?, pNorm: Float?, scalesGradientByFrequency: Bool)

Creates an embedding descriptor with the size and dimension of embedding vectors, padding index, and norm and scaling options that you specify.

Deprecated

