

- Accelerate
-  BNNSNormType 

Structure

# BNNSNormType

Constants that describe norm types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSNormType
```

## Topics

### Constants

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSL2Norm: BNNSNormType

A constant that represents the L2 norm.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Compute norm functions

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

func BNNSComputeNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Computes the specified norm over an entire tensor or the specified axes.

Deprecated

func BNNSComputeNormBackward(UnsafeRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafeRawPointer, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Backpropogates gradients for the compute norm function.

Deprecated

