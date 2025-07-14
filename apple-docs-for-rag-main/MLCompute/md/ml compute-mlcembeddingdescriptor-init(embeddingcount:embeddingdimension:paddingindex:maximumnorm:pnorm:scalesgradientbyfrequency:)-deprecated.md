

- ML Compute
- MLCEmbeddingDescriptor
-  init(embeddingCount:embeddingDimension:paddingIndex:maximumNorm:pNorm:scalesGradientByFrequency:) Deprecated

Initializer

# init(embeddingCount:embeddingDimension:paddingIndex:maximumNorm:pNorm:scalesGradientByFrequency:)

Creates an embedding descriptor with the size and dimension of embedding vectors, padding index, and norm and scaling options that you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    embeddingCount: Int,
    embeddingDimension: Int,
    paddingIndex: Int?,
    maximumNorm: Float?,
    pNorm: Float?,
    scalesGradientByFrequency: Bool
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`embeddingCount`  

The size of the dictionary.

`embeddingDimension`  

The dimension of embedding vectors.

`paddingIndex`  

An unsigned integer value. If set, the layer initializes the embedding vector at that index to zero, and won’t update the vector in the gradient pass. The default value is `nil`.

`maximumNorm`  

A float value. If set, the layer renormalizes the selected embedding vectors in the forward pass only to have an Lp norm less than this value. The default value is `nil`.

`pNorm`  

A float value that specifies the p of the Lp norm. The default value is `2.0`.

`scalesGradientByFrequency`  

A Boolean value that indicates whether you scale the gradients by the inverse of the frequency of words in batch before the weight update. The default value is `false`.

## See Also

### Creating Embedding Descriptors

convenience init?(embeddingCount: Int, embeddingDimension: Int)

Creates an embedding descriptor with the size of the dictionary and dimension of embedding vectors you specify.

Deprecated

