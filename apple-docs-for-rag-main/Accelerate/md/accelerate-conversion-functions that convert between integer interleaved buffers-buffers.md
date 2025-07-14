

- Accelerate
- Conversion
-  Functions that convert between integer interleaved buffers 

API Collection

# Functions that convert between integer interleaved buffers

Convert the bit depths of interleaved integer image data.

## Topics

### Converting from 8-bit buffers

func vImageConvert_RGB888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 3-channel interleaved buffer to an RGB565 3-channel interleaved buffer using the specified dithering algorithm.

func vImageConvert_ARGB8888toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer.

func vImageConvert_ARGB8888toARGB1555_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_RGBA8888toRGBA5551(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer.

func vImageConvert_RGBA8888toRGBA5551_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_ARGB8888ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel buffer with permutation.

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_RGB16UtoRGB888_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 3-channel interleaved buffer to an 8-bit-per-channel, 3-channel interleaved buffer using the specified dithering algorithm.

func vImageConvert_ARGB16UToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_ARGB16UtoARGB8888_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer using the specified dithering algorithm.

### Converting from RGB565 16-bit-per-channel buffers

func vImageConvert_RGB565toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an RGB565 3-channel interleaved buffer to an 8-bit-per-channel, 3-channel interleaved buffer.

### Converting from ARGB1555 16-bit-per-channel buffers

func vImageConvert_RGBA5551toRGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an RGB5651 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_ARGB1555toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an ARGB1555 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer.

## See Also

### Type conversion

Functions that convert between integer planar buffers

Convert the bit depths of planar integer image data.

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

