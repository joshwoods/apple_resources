

- Accelerate
- BNNS
- BNNS.EmbeddingLayer
-  init(input:output:dictionary:paddingIndex:maximumNorm:normType:scalesGradientByFrequency:filterParameters:) Deprecated

Initializer

# init(input:output:dictionary:paddingIndex:maximumNorm:normType:scalesGradientByFrequency:filterParameters:)

Returns a new embedding layer.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    dictionary: BNNSNDArrayDescriptor,
    paddingIndex: Int,
    maximumNorm: Float,
    normType: BNNS.Norm,
    scalesGradientByFrequency: Bool,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`dictionary`  

The descriptor of the dictionary array.

`paddingIndex`  

The padding index. The operation returns a zero tensor for dictionary items with an index that corresponds to the padding index.

`maximumNorm`  

The maximum norm. If nonzero, the operation renormalizes any vector with a norm greater than `maximumNorm` during forward lookups

`normType`  

The norm type. If `normType` is nonzero, this value specifies the p-norm where p equals `norm_type`.

`scalesGradientByFrequency`  

A Boolean value that specifies that the operation scales calculated gradients based on the number of occurrence of the corresponding index in the input.

`filterParameters`  

The filter runtime parameters.

## See Also

### Related Documentation

func BNNSFilterCreateLayerEmbedding(UnsafePointer&lt;BNNSLayerParametersEmbedding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new embedding layer.

Deprecated

### Creating an Embedding Layer

struct Norm

Constants that describe norm types.

Deprecated

