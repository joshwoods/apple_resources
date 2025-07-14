

- Accelerate
- Conversion
-  Functions that convert from noninteger interleaved buffers to integer interleaved buffers 

API Collection

# Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

## Topics

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_RGBFFFtoRGB888_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, UnsafePointer&lt;Pixel_F>, Int32, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit-per-channel, 3-channel buffer to an 8-bit-per-channel, 3-channel buffer using the specified dithering algorithm.

func vImageConvert_ARGBFFFFtoARGB8888_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit-per-channel, 4-channel buffer to an 8-bit-per-channel, 4-channel buffer using the specified dithering algorithm.

### Converting from XRGB2101010 32-bit buffers

func vImageConvert_ARGB2101010ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an ARGB2101010 32-bit, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_XRGB2101010ToARGB8888(UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an XRGB2101010 32-bit, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_ARGB2101010ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an ARGB2101010 32-bit, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_XRGB2101010ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UInt16, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an XRGB2101010 32-bit, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel interleaved buffer with permutation.

### Converting from RGBX1010102 32-bit buffers

func vImageConvert_RGBA1010102ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an RGBA1010102 32-bit, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_RGBA1010102ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an RGBA1010102 32-bit, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel interleaved buffer with permutation.

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

Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

