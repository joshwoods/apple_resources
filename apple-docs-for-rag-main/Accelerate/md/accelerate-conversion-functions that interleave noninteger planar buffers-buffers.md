

- Accelerate
- Conversion
-  Functions that interleave noninteger planar buffers 

API Collection

# Functions that interleave noninteger planar buffers

Combine discrete fixed- and floating-point planar buffers into an interleaved buffer.

## Topics

### Interleaving three fixed-point 16-bit planar buffers

func vImageConvert_Planar16Q12toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three fixed-point 16-bit planar buffers into an 8-bit-per-channel, 3-channel interleaved buffer.

func vImageConvert_Planar16Q12toRGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three fixed-point 16-bit planar buffers into a floating-point 32-bit-per-channel, 3-channel interleaved buffer.

### Interleaving four fixed-point 16-bit planar buffers

func vImageConvert_Planar16Q12toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four fixed-point 16-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_Planar16Q12toARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four fixed-point 16-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

### Interleaving floating-point 32-bit planar buffers

func vImageConvert_PlanarToChunkyF(UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, UInt32, Int, vImagePixelCount, vImagePixelCount, Int, vImage_Flags) -> vImage_Error

Interleaves the specifed number of floating-point 32-bit planar buffers into a floating-point 32 -bit-per-channel interleaved buffer.

### Interleaving three floating-point 32-bit planar buffers

func vImageConvert_PlanarFToBGRX8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Interleaves three 32-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

vImageConvert_PlanarFToRGBX8888

Interleaves three 32-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved RGBX buffer with the specified constant alpha value.

func vImageConvert_PlanarFToXRGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Interleaves three 32-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

func vImageConvert_PlanarFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three floating-point 32-bit planar buffers into a floating-point 32-bit-per-channel, 3-channel interleaved buffer.

vImageConvert_PlanarFToRGBXFFFF

Interleaves three 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved RGBX buffer with the specified constant alpha value.

func vImageConvert_PlanarFToXRGBFFFF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

### Interleaving four floating-point 32-bit planar buffers

func vImageConvert_PlanarFToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Interleaves four 32-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_PlanarFtoARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four floating-point 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel ARGB interleaved buffer.

func vImageConvert_PlanarFToBGRXFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four floating-point 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel BGRXARGB interleaved buffer.

## See Also

### Converting between interleaved and planar formats

Functions that interleave integer planar buffers

Combine discrete integer planar buffers into an interleaved buffer.

Functions that deinterleave integer interleaved buffers

Separate integer interleaved buffers into discrete planar buffers.

Functions that deinterleave noninteger interleaved buffers

Separate fixed- and floating-point interleaved buffers into discrete planar buffers.

