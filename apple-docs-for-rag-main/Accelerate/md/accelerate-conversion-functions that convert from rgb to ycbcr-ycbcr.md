

- Accelerate
- Conversion
-  Functions that convert from RGB to YCbCr 

API Collection

# Functions that convert from RGB to YCbCr

Convert image data represented by red, green, and blue channels to luma, blue-difference, and red-difference channels.

## Topics

### Converting to 4:2:0

func vImageConvert_ARGB8888To420Yp8_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to a planar Yp buffer and a 2-channel CbCr buffer.

func vImageConvert_ARGB8888To420Yp8_Cb8_Cr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to planar Yp, Cb, and Cr buffers.

### Converting to 4:2:2

func vImageConvert_ARGB8888To422CbYpCrYp8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:2:2 CbCrYp buffer.

func vImageConvert_ARGB8888To422YpCbYpCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:2:2 YpCbYpCr buffer.

func vImageConvert_ARGB8888To422CbYpCrYp8_AA8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:2:2 CbYpCrYp buffer and an 8-bit alpha buffer.

func vImageConvert_ARGB8888To422CbYpCrYp16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to a 16-bit-per-channel 4:2:2 CbYpCrYp buffer.

func vImageConvert_ARGB8888To422CrYpCbYpCbYpCbYpCrYpCrYp10(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to a 10-bit-per-channel 4:2:2 CrYpCbYpCbYpCbYpCrYpCrYp buffer.

func vImageConvert_ARGB16UTo422CbYpCrYp16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel ARGB buffer to a 16-bit-per-channel 4:2:2 CbYpCrYp buffer.

func vImageConvert_ARGB16Q12To422CrYpCbYpCbYpCbYpCrYpCrYp10(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit-per-channel, 4-channel ARGB buffer to a 10-bit-per-channel 4:2:2 CrYpCbYpCbYpCbYpCrYpCrYp buffer.

### Converting to 4:4:4

func vImageConvert_ARGB8888To444CrYpCb8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:4:4 CrYpCb buffer.

func vImageConvert_ARGB8888To444AYpCbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:4:4 YpCbCr buffer.

func vImageConvert_ARGB8888To444CbYpCrA8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 8-bit-per-channel 4:4:4 CrYpCbA buffer.

func vImageConvert_ARGB8888To444CrYpCb10(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 10-bit-per-channel 4:4:4 CrYpCb buffer.

func vImageConvert_ARGB8888To444AYpCbCr16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to an 16-bit-per-channel 4:4:4 YpCbCr buffer.

func vImageConvert_ARGB16UTo444AYpCbCr16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel ARGB buffer to an 16-bit-per-channel 4:4:4 AYpCbCr buffer.

func vImageConvert_ARGB16Q12To444CrYpCb10(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit-per-channel, 4-channel ARGB buffer to an 10-bit-per-channel 4:4:4 CrYpCb buffer.

### Generating conversion information

func vImageConvert_ARGBToYpCbCr_GenerateConversion(UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>, UnsafePointer&lt;vImage_YpCbCrPixelRange>, UnsafeMutablePointer&lt;vImage_ARGBToYpCbCr>, vImageARGBType, vImageYpCbCrType, vImage_Flags) -> vImage_Error

Generates the information that describes the conversion from ARGB to YpCbCr.

struct vImageYpCbCrType

Constants that describe the encoding of a YpCbCr image for conversions between RGB and YpCbCr.

struct vImageARGBType

Constants that describe the encoding of an ARGB image for conversions between RGB and YpCbCr.

struct vImage_ARGBToYpCbCrMatrix

The 3 x 3 matrix that the vImage library uses to convert from RGB to YpCbCr.

struct vImage_ARGBToYpCbCr

The information that describes the conversion from ARGB to YpCbCr.

struct vImage_YpCbCrPixelRange

The description of range and clamping information for YpCbCr pixel formats.

## See Also

### Converting between YCbCr and RGB color spaces

Functions that convert from YCbCr to RGB

Convert image data represented by luma, blue-difference, and red-difference channels to red, green, and blue channels.

