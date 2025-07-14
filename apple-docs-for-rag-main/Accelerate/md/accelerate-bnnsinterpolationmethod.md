

- Accelerate
-  BNNSInterpolationMethod 

Structure

# BNNSInterpolationMethod

Constants that describe interpolation methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSInterpolationMethod
```

## Topics

### Interpolation Methods

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

var BNNSInterpolationMethodLinear: BNNSInterpolationMethod

Interpolation that is linear or bilinear depending on the number of resized dimensions.

var BNNSInterpolationMethodNearest: BNNSInterpolationMethod

Nearest-neighbor interpolation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Resize layers

class ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersResize

A structure that contains the parameters of a resize layer.

Deprecated

func BNNSFilterCreateLayerResize(UnsafePointer&lt;BNNSLayerParametersResize>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new resize layer.

Deprecated

