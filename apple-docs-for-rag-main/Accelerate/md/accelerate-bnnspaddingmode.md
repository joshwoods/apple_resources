

- Accelerate
-  BNNSPaddingMode 

Structure

# BNNSPaddingMode

Constants that define padding modes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSPaddingMode
```

## Topics

### Padding Modes

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSPaddingModeConstant: BNNSPaddingMode

A constant that indicates that a padding operation fills the padded area with a specified constant.

var BNNSPaddingModeReflect: BNNSPaddingMode

A constant that indicates that a padding operation fills the padded area to form an odd-symmetric pattern.

var BNNSPaddingModeSymmetric: BNNSPaddingMode

A constant that indicates that a padding operation fills the padded area to form an even-symmetric pattern.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Padding layers

class PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersPadding

A structure that contains the parameters of a padding layer.

Deprecated

func BNNSFilterCreateLayerPadding(UnsafePointer&lt;BNNSLayerParametersPadding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

