

- Accelerate
- BNNSLayerParametersEmbedding
-  init(flags:i_desc:o_desc:dictionary:padding_idx:max_norm:norm_type:) Deprecated

Initializer

# init(flags:i_desc:o_desc:dictionary:padding_idx:max_norm:norm_type:)

Returns a new embedding layer parameter structure from the specified parameters.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
init(
    flags: BNNSEmbeddingFlags,
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    dictionary: BNNSNDArrayDescriptor,
    padding_idx: Int,
    max_norm: Float,
    norm_type: Float
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`flags`  

A bit field for flags that specify additional behavior, such as scaling gradient by frequency.

`i_desc`  

The signed or unsigned integer descriptor of the input.

`o_desc`  

The descriptor of the output.

`dictionary`  

The descriptor of the dictionary.

`padding_idx`  

The padding index. The operation returns a zero tensor for dictionary items with an index that corresponds to the padding index.

`max_norm`  

The maximum norm. If nonzero, the operation renormalizes any vector with a norm greater than `max_norm` during forward lookups.

`norm_type`  

The norm type. If `max_norm` is nonzero, this value specifies the p-norm where `p = norm_type`.

## See Also

### Initializers

init()

Returns a new embedding layer parameters structure.

Deprecated

