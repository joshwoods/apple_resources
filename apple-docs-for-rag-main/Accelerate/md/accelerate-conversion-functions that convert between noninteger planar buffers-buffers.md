

- Accelerate
- Conversion
-  Functions that convert between noninteger planar buffers 

API Collection

# Functions that convert between noninteger planar buffers

Convert the bit depths and formats of planar fixed- and floating-point image data.

## Topics

### Converting from floating-point 16-bit-per-channel buffers

func vImageConvert_16Fto16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 16-bit planar buffer to a fixed-point 16-bit planar buffer.

func vImageConvert_Planar16FtoPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 16-bit planar buffer to a floating-point 32-bit planar buffer.

### Converting from fixed-point 16-bit-per-channel buffers

func vImageConvert_16Q12to16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit planar buffer to a floating-point 16-bit planar buffer.

func vImageConvert_16Q12toF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit planar buffer to a floating-point 32-bit planar buffer.

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_PlanarFtoPlanar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to a floating-point 16-bit planar buffer.

func vImageConvert_Fto16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to a fixed-point 16-bit planar buffer.

## See Also

### Type conversion

Functions that convert between integer planar buffers

Convert the bit depths of planar integer image data.

Functions that convert between integer interleaved buffers

Convert the bit depths of interleaved integer image data.

Functions that convert from integer planar buffers to noninteger planar buffers

Convert planar integer image data to fixed- and floating-point format.

Functions that convert from integer interleaved buffers to noninteger interleaved buffers

Convert interleaved integer image data to fixed- and floating-point format.

Functions that convert between noninteger interleaved buffers

Convert the bit depths and formats of interleaved fixed- and floating-point image data.

Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

