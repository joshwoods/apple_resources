

- Accelerate
- BNNSLayerParametersEmbedding
-  flags Deprecated

Instance Property

# flags

A bit field for flags that specify additional behavior, such as scaling gradient by frequency.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
var flags: BNNSEmbeddingFlags
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

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

var norm_type: Float

The norm type.

Deprecated

