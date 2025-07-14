

- Accelerate
-  BNNSEmbeddingFlags 

Structure

# BNNSEmbeddingFlags

Flags that control behavior of embedding layers.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSEmbeddingFlags
```

## Topics

### Embedding Flags

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSEmbeddingFlagScaleGradientByFrequency: BNNSEmbeddingFlags

A flag that specifies that the operation scales calculated gradients based on the number of occurrence of the corresponding index in the input.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Instance Properties

var flags: BNNSEmbeddingFlags

A bit field for flags that specify additional behavior, such as scaling gradient by frequency.

Deprecated

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

