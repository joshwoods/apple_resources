

- Accelerate
-  BNNSShuffleType 

Structure

# BNNSShuffleType

Constants that specify a shuffle type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSShuffleType
```

## Topics

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSShuffleTypePixelShuffleNCHW: BNNSShuffleType

The pixel shuffle for the NCHW (batch, channels, height, width) format, equivalent to depth-to-space in Column Row Depth (CRD) mode.

var BNNSShuffleTypePixelUnshuffleNCHW: BNNSShuffleType

The pixel unshuffle for the NCHW (batch, channels, height, width) format, equivalent to space-to-depth in Column Row Depth (CRD) mode.

var BNNSShuffleTypeDepthToSpaceNCHW: BNNSShuffleType

var BNNSShuffleTypeSpaceToDepthNCHW: BNNSShuffleType

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

enum Error

func BNNSBandPart(Int32, Int32, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

func BNNSShuffle(BNNSShuffleType, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Rearranges elements in a tensor according to shuffle type.

Deprecated

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

