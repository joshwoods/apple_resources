

- ML Compute
-  MLCMultiheadAttentionDescriptor Deprecated

Class

# MLCMultiheadAttentionDescriptor

A configuration object you use to create a multi-head attention layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCMultiheadAttentionDescriptor
```

## Topics

### Creating Multi-Head Attention Descriptors

convenience init(modelDimension: Int, headCount: Int)

Creates a multi-head attention descriptor with the model dimension and number of parallel attention heads you specify.

convenience init?(modelDimension: Int, keyDimension: Int, valueDimension: Int, headCount: Int, dropout: Float, hasBiases: Bool, hasAttentionBiases: Bool, addsZeroAttention: Bool)

Creates a multi-head attention descriptor with the dimensions, number of attention heads, dropout rate, and bias and padding options you specify.

### Inspecting Multi-Head Attention Descriptors

var modelDimension: Int

The model or embedding dimension.

var keyDimension: Int

The total dimension of key space, which must be divisible by the number of heads.

var valueDimension: Int

The total dimension of value space, which must be divisible by the number of heads.

var headCount: Int

The number of parallel attention heads.

var dropout: Float

The dropout rate you apply to the output projection weights.

var hasBiases: Bool

A Boolean that specifies whether you add a bias to query, key, value, and output projections.

var hasAttentionBiases: Bool

A Boolean that specifies whether you add an array of biases to key and value, respectively.

var addsZeroAttention: Bool

A Boolean that specifies whether you add a row of zeros to projected key and value.

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

### Creating Multi-Head Attention Layers

convenience init?(descriptor: MLCMultiheadAttentionDescriptor, weights: [MLCTensor], biases: [MLCTensor]?, attentionBiases: [MLCTensor]?)

Creates a multi-head attention layer with the descriptor, weights, and biases you specify.

Deprecated

