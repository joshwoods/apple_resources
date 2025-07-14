

- Accelerate
- BNNSLayerParametersEmbedding
-  norm_type Deprecated

Instance Property

# norm_type

The norm type.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
var norm_type: Float
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

If `max_norm` is nonzero, this value specifies the p-norm where `p = norm_type`.

## See Also

### Instance Properties

var flags: BNNSEmbeddingFlags

A bit field for flags that specify additional behavior, such as scaling gradient by frequency.

Deprecated

struct BNNSEmbeddingFlags

Flags that control behavior of embedding layers.

var i_desc: BNNSNDArrayDescriptor

The signed or unsigned integer descriptor of the input.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

var dictionary: BNNSNDArrayDescriptor

The descriptor of the dictionary.

Deprecated

var padding_idx: Int

The padding index.

Deprecated

var max_norm: Float

The maximum norm.

Deprecated

