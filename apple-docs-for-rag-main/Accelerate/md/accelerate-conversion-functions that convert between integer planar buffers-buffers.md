

- Accelerate
- Conversion
-  Functions that convert between integer planar buffers 

API Collection

# Functions that convert between integer planar buffers

Convert the bit depths of planar integer image data.

## Topics

### Converting from 1-bit buffers

func vImageConvert_Planar1toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a 1-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_Indexed1toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Converts an indexed 1-bit planar buffer to an 8-bit planar buffer.

### Converting from 2-bit buffers

func vImageConvert_Planar2toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a 2-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_Indexed2toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Converts an indexed 2-bit planar buffer to an 8-bit planar buffer.

### Converting from 4-bit buffers

func vImageConvert_Planar4toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a 4-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_Indexed4toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Converts an indexed 4-bit planar buffer to an 8-bit planar buffer.

### Converting from 8-bit buffers

func vImageConvert_Planar8toPlanar1(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a 1-bit planar buffer.

func vImageConvert_Planar8toPlanar2(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a 2-bit planar buffer.

func vImageConvert_Planar8toPlanar4(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a 4-bit planar buffer.

func vImageConvert_Planar8toIndexed1(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 1-bit planar buffer.

func vImageConvert_Planar8toIndexed2(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 2-bit planar buffer.

func vImageConvert_Planar8toIndexed4(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 4-bit planar buffer.

func vImageConvert_Planar8To16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an unsigned 16-bit planar buffer.

### Converting from unsigned 12-bit-per-channel buffers

func vImageConvert_12UTo16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 12-bit planar buffer to an unsigned 16-bit planar buffer.

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_16UToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_Planar16UtoPlanar8_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to an 8-bit planar buffer using the specified dithering algorithm.

func vImageConvert_16UTo12U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to an unsigned 12-bit planar buffer.

## See Also

### Type conversion

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

Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

