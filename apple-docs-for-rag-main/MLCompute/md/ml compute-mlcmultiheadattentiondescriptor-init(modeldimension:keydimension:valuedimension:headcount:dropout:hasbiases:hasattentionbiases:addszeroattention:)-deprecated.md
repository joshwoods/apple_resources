

- ML Compute
- MLCMultiheadAttentionDescriptor
-  init(modelDimension:keyDimension:valueDimension:headCount:dropout:hasBiases:hasAttentionBiases:addsZeroAttention:) Deprecated

Initializer

# init(modelDimension:keyDimension:valueDimension:headCount:dropout:hasBiases:hasAttentionBiases:addsZeroAttention:)

Creates a multi-head attention descriptor with the dimensions, number of attention heads, dropout rate, and bias and padding options you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    modelDimension: Int,
    keyDimension: Int,
    valueDimension: Int,
    headCount: Int,
    dropout: Float,
    hasBiases: Bool,
    hasAttentionBiases: Bool,
    addsZeroAttention: Bool
)
```

## Parameters 

`modelDimension`  

The total dimension of model space.

`keyDimension`  

The total dimension of key space; the default value is equal to `modelDimension`.

`valueDimension`  

The total dimension of value space; the default value is equal to `modelDimension`.

`headCount`  

The number of parallel attention heads.

`dropout`  

The dropout rate you apply to the output projection weights; the default value is `0.0`.

`hasBiases`  

A Boolean that specifies whether you add a bias to query, key, value, and output projections; the default value is `true`.

`hasAttentionBiases`  

A Boolean that specifies whether you add a row of zeros to projected key and value; the default value is `false`.

`addsZeroAttention`  

A Boolean that specifies whether you add a row of zeros to projected key and value; the default value is `false`.

## See Also

### Creating Multi-Head Attention Descriptors

convenience init(modelDimension: Int, headCount: Int)

Creates a multi-head attention descriptor with the model dimension and number of parallel attention heads you specify.

Deprecated

