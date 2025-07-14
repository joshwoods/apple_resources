

- Accelerate
-  BNNSFilterType 

Structure

# BNNSFilterType

Constants that define the component filters of a fused layer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSFilterType
```

## Topics

### Layer Constants

var BNNSArithmetic: BNNSFilterType

An arithmetic filter.

var BNNSConvolution: BNNSFilterType

A convolution filter.

var BNNSTransposedConvolution: BNNSFilterType

A transposed convolution filter.

var BNNSFullyConnected: BNNSFilterType

A fully connected filter.

var BNNSBatchNorm: BNNSFilterType

A batch normalization filter.

var BNNSGroupNorm: BNNSFilterType

A group normalization filter.

var BNNSInstanceNorm: BNNSFilterType

An instance normalization filter.

var BNNSLayerNorm: BNNSFilterType

A layer normalization filter.

var BNNSQuantization: BNNSFilterType

A quantization filter.

### Raw Values

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

Deprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

func BNNSFilterCreateFusedLayer(Int, UnsafePointer&lt;BNNSFilterType>, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fused layer.

Deprecated

func BNNSFusedFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a multiple-input fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a fused filter backward to generate input gradients.

Deprecated

func BNNSFusedFilterApplyBackwardMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a multiple-input fused filter backward to generate input gradients.

Deprecated

