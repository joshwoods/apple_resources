

- Accelerate
-  vImageARGBType 

Structure

# vImageARGBType

Constants that describe the encoding of an ARGB image for conversions between RGB and YpCbCr.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImageARGBType
```

## Topics

### Constants

init(UInt32)

Creates a new ARGB type.

init(rawValue: UInt32)

Creates a new ARGB type with an unsigned integer value.

var rawValue: UInt32

The unsigned integer raw value.

var kvImageARGB16Q12: vImageARGBType

Any 8-bit four-channel interleaved buffer.

var kvImageARGB16U: vImageARGBType

Any 16-bit unsigned, four-channel interleaved buffer.

var kvImageARGB8888: vImageARGBType

Any 16-bit signed fixed-point, four-channel interleaved buffer.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Generating conversion information

func vImageConvert_ARGBToYpCbCr_GenerateConversion(UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>, UnsafePointer&lt;vImage_YpCbCrPixelRange>, UnsafeMutablePointer&lt;vImage_ARGBToYpCbCr>, vImageARGBType, vImageYpCbCrType, vImage_Flags) -> vImage_Error

Generates the information that describes the conversion from ARGB to YpCbCr.

struct vImageYpCbCrType

Constants that describe the encoding of a YpCbCr image for conversions between RGB and YpCbCr.

struct vImage_ARGBToYpCbCrMatrix

The 3 x 3 matrix that the vImage library uses to convert from RGB to YpCbCr.

struct vImage_ARGBToYpCbCr

The information that describes the conversion from ARGB to YpCbCr.

struct vImage_YpCbCrPixelRange

The description of range and clamping information for YpCbCr pixel formats.

