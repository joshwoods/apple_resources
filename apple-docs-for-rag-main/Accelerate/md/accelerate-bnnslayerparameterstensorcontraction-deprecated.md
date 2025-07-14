

- Accelerate
-  BNNSLayerParametersTensorContraction Deprecated

Structure

# BNNSLayerParametersTensorContraction

A structure that contains the parameters of a tensor-contraction layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersTensorContraction
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(operation: UnsafePointer&lt;CChar>, alpha: Float, beta: Float, iA_desc: BNNSNDArrayDescriptor, iB_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor)

Returns a new tensor-contraction parameters structure.

### Instance Properties

var operation: UnsafePointer&lt;CChar>

The string that describes the operation.

var alpha: Float

Scaling that the operation applies to the result.

var beta: Float

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

var iA_desc: BNNSNDArrayDescriptor

The descriptor of input matrix *A*.

var iB_desc: BNNSNDArrayDescriptor

The descriptor of input matrix *B*.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Tensor contraction layers

func BNNSFilterCreateLayerTensorContraction(UnsafePointer&lt;BNNSLayerParametersTensorContraction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new tensor-contraction layer.

Deprecated

