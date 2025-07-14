

- ML Compute
- MLCMultiheadAttentionDescriptor
-  init(modelDimension:headCount:) Deprecated

Initializer

# init(modelDimension:headCount:)

Creates a multi-head attention descriptor with the model dimension and number of parallel attention heads you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    modelDimension: Int,
    headCount: Int
)
```

## Parameters 

`modelDimension`  

The total dimension of model space.

`headCount`  

The number of parallel attention heads.

## See Also

### Creating Multi-Head Attention Descriptors

convenience init?(modelDimension: Int, keyDimension: Int, valueDimension: Int, headCount: Int, dropout: Float, hasBiases: Bool, hasAttentionBiases: Bool, addsZeroAttention: Bool)

Creates a multi-head attention descriptor with the dimensions, number of attention heads, dropout rate, and bias and padding options you specify.

Deprecated

