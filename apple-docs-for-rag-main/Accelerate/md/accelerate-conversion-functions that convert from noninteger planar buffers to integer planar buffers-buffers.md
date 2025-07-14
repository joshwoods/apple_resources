

- Accelerate
- Conversion
-  Functions that convert from noninteger planar buffers to integer planar buffers 

API Collection

# Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

## Topics

### Converting from fixed-point 16-bit-per-channel buffers

func vImageConvert_16Q12to8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_16Q12to16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a fixed-point 16-bit planar buffer to an unsigned 16-bit planar buffer.

### Converting from floating-point 16-bit-per-channel buffers

func vImageConvert_Planar16FtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floaing-point 16-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_16Fto16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 16-bit planar buffer to an unsigned 16-bit planar buffer.

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_PlanarFtoPlanar8_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, Pixel_F, Int32, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to an 8-bit planar buffer using the specified dithering algorithm.

func vImageConvert_FTo16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to a signed 16-bit planar buffer.

func vImageConvert_FTo16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to an unsigned 16-bit planar buffer.

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

Functions that convert between noninteger planar buffers

Convert the bit depths and formats of planar fixed- and floating-point image data.

Functions that convert between noninteger interleaved buffers

Convert the bit depths and formats of interleaved fixed- and floating-point image data.

Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

