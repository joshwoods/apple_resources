

- Accelerate
- Conversion
-  Functions that interleave integer planar buffers 

API Collection

# Functions that interleave integer planar buffers

Combine discrete integer planar buffers into an interleaved buffer.

## Topics

### Interleaving unsigned 8-bit planar buffers

func vImageConvert_PlanarToChunky8(UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, UInt32, Int, vImagePixelCount, vImagePixelCount, Int, vImage_Flags) -> vImage_Error

Interleaves the specifed number of 8-bit planar buffers into an 8-bit-per-channel interleaved buffer.

### Interleaving three unsigned 8-bit planar buffers

func vImageConvert_Planar8toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an RGB565 3-channel interleaved buffer.

func vImageConvert_Planar8toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 3-channel interleaved buffer.

func vImageConvert_Planar8ToXRGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

vImageConvert_Planar8ToRGBX8888

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved RGBX buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRX8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

func vImageConvert_Planar8ToXRGBFFFF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRXFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

vImageConvert_Planar8ToRGBXFFFF

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved RGBX buffer with the specified constant alpha value.

### Interleaving four unsigned 8-bit planar buffers

func vImageConvert_Planar8toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four 8-bit planar buffers into an ARGB1555 4-channel interleaved buffer.

func vImageConvert_Planar8toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_Planar8ToARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves four 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved ARGB buffer.

### Interleaving three unsigned 16-bit planar buffers

func vImageConvert_Planar16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three unsigned 16-bit planar buffers into an unsigned 16-bit-per-channel, 3-channel interleaved buffer.

### Interleaving four unsigned 16-bit planar buffers

func vImageConvert_Planar16UtoARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four unsigned 16-bit planar buffers into an unsigned 16-bit-per-channel, 4-channel interleaved ARGB buffer.

## See Also

### Converting between interleaved and planar formats

Functions that interleave noninteger planar buffers

Combine discrete fixed- and floating-point planar buffers into an interleaved buffer.

Functions that deinterleave integer interleaved buffers

Separate integer interleaved buffers into discrete planar buffers.

Functions that deinterleave noninteger interleaved buffers

Separate fixed- and floating-point interleaved buffers into discrete planar buffers.

