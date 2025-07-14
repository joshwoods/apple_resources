

- Accelerate
-  BNNSMHAProjectionParameters 

Structure

# BNNSMHAProjectionParameters

A structure that contains multihead attention projection parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSMHAProjectionParameters
```

## Topics

### Initializers

init(target_desc: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor)

Returns a new multihead attention projection parameters structure from the specified parameters.

init()

Returns a new multihead attention projection parameters structure.

### Instance Properties

var target_desc: BNNSNDArrayDescriptor

The descriptor—which is either an input query, key, or value, or an output—of the main target of the operation.

var weights: BNNSNDArrayDescriptor

The descriptor of the initial projection’s weights.

var bias: BNNSNDArrayDescriptor

The descriptor of the initial projection’s bias.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Multihead attention layers

struct BNNSLayerParametersMultiheadAttention

A structure that contains the parameters of a multihead attention layer.

Deprecated

func BNNSFilterCreateLayerMultiheadAttention(UnsafePointer&lt;BNNSLayerParametersMultiheadAttention>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new multihead attention layer.

Deprecated

func BNNSApplyMultiheadAttention(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSApplyMultiheadAttentionBackward(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>, Int, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a multihead attention filter backward to generate gradients.

Deprecated

