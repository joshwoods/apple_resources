

- Accelerate
- BNNS
-  BNNS.Error 

Enumeration

# BNNS.Error

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum Error
```

## Topics

### Enumeration Cases

case arrayDescriptorInvalidData

case layerApplyFail

case optimizerStepFail

case unableToCreateLayer

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

func BNNSBandPart(Int32, Int32, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

func BNNSShuffle(BNNSShuffleType, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Rearranges elements in a tensor according to shuffle type.

Deprecated

struct BNNSShuffleType

Constants that specify a shuffle type.

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

