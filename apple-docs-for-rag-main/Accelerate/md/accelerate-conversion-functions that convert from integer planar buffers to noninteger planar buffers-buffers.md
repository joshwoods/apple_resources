

- Accelerate
- Conversion
-  Functions that convert from integer planar buffers to noninteger planar buffers 

API Collection

# Functions that convert from integer planar buffers to noninteger planar buffers

Convert planar integer image data to fixed- and floating-point format.

## Topics

### Converting from 8-bit buffers

func vImageConvert_8to16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a fixed-point 16-bit planar buffer.

func vImageConvert_Planar8toPlanar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a floating-point 16-bit planar buffer.

func vImageConvert_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a floating-point 32-bit planar buffer.

### Converting from signed 16-bit-per-channel buffers

func vImageConvert_16SToF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts a signed 16-bit planar buffer to a floating-point 32-bit planar buffer.

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_16Uto16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to a floating-point 16-bit planar buffer.

func vImageConvert_16Uto16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to a fixed-point 16-bit planar buffer.

func vImageConvert_16UToF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to a floating-point 32-bit planar buffer.

## See Also

### Type conversion

Functions that convert between integer planar buffers

Convert the bit depths of planar integer image data.

Functions that convert between integer interleaved buffers

Convert the bit depths of interleaved integer image data.

Functions that convert from integer interleaved buffers to noninteger interleaved buffers

Convert interleaved integer image data to fixed- and floating-point format.

Functions that convert between noninteger planar buffers

Convert the bit depths and formats of planar fixed- and floating-point image data.

Functions that convert between noninteger interleaved buffers

Convert the bit depths and formats of interleaved fixed- and floating-point image data.

Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

