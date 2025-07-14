

- Accelerate
-  BNNSLayerParametersEmbedding Deprecated

Structure

# BNNSLayerParametersEmbedding

A structure that contains the parameters of an embedding layer.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
struct BNNSLayerParametersEmbedding
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init()

Returns a new embedding layer parameters structure.

init(flags: BNNSEmbeddingFlags, i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, dictionary: BNNSNDArrayDescriptor, padding_idx: Int, max_norm: Float, norm_type: Float)

Returns a new embedding layer parameter structure from the specified parameters.

### Instance Properties

var flags: BNNSEmbeddingFlags

A bit field for flags that specify additional behavior, such as scaling gradient by frequency.

struct BNNSEmbeddingFlags

Flags that control behavior of embedding layers.

var i_desc: BNNSNDArrayDescriptor

The signed or unsigned integer descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var dictionary: BNNSNDArrayDescriptor

The descriptor of the dictionary.

var padding_idx: Int

The padding index.

var max_norm: Float

The maximum norm.

var norm_type: Float

The norm type.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Embedding layers

class EmbeddingLayer

A layer object that wraps an embedding filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerEmbedding(UnsafePointer&lt;BNNSLayerParametersEmbedding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new embedding layer.

Deprecated

