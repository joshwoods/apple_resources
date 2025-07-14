

- ML Compute
- MLCMultiheadAttentionDescriptor
-  modelDimension Deprecated

Instance Property

# modelDimension

The model or embedding dimension.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var modelDimension: Int { get }
```

## See Also

### Inspecting Multi-Head Attention Descriptors

var keyDimension: Int

The total dimension of key space, which must be divisible by the number of heads.

Deprecated

var valueDimension: Int

The total dimension of value space, which must be divisible by the number of heads.

Deprecated

var headCount: Int

The number of parallel attention heads.

Deprecated

var dropout: Float

The dropout rate you apply to the output projection weights.

Deprecated

var hasBiases: Bool

A Boolean that specifies whether you add a bias to query, key, value, and output projections.

Deprecated

var hasAttentionBiases: Bool

A Boolean that specifies whether you add an array of biases to key and value, respectively.

Deprecated

var addsZeroAttention: Bool

A Boolean that specifies whether you add a row of zeros to projected key and value.

Deprecated

