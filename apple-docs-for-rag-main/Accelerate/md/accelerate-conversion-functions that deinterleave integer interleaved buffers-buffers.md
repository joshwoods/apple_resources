

- Accelerate
- Conversion
-  Functions that deinterleave integer interleaved buffers 

API Collection

# Functions that deinterleave integer interleaved buffers

Separate integer interleaved buffers into discrete planar buffers.

## Topics

### Deinterleaving unsigned 8-bit interleaved buffers

func vImageConvert_ChunkyToPlanar8(UnsafeMutablePointer&lt;UnsafeRawPointer?>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UInt32, Int, vImagePixelCount, vImagePixelCount, Int, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel interleaved buffer with an arbitrary number of channels into the corresponding number of 8-bit planar buffers.

### Deinterleaving unsigned 8-bit, three-channel interleaved buffers

func vImageConvert_RGB888toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 3-channel interleaved buffer into three 8-bit planar buffers.

func vImageConvert_RGB888toPlanar16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 3-channel interleaved buffer into three fixed-point 16-bit planar buffers.

### Deinterleaving unsigned 8-bit, four-channel interleaved buffers

func vImageConvert_BGRX8888ToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into three 8-bit planar buffers and discards the last channel.

func vImageConvert_XRGB8888ToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into three 8-bit planar buffers and discards the first channel.

func vImageConvert_ARGB8888toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four 8-bit planar buffers.

func vImageConvert_ARGB8888toPlanar16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four fixed-point 16-bit planar buffers.

func vImageConvert_ARGB8888toPlanarF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four floating-point 32-bit planar buffers.

### Deinterleaving unsigned 16-bit three-channel interleaved buffers

func vImageConvert_RGB16UtoPlanar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an unsigned 16-bit-per-channel, 3-channel interleaved buffer into three unsigned 16-bit planar buffers.

### Deinterleaving unsigned 16-bit four-channel interleaved buffers

func vImageConvert_ARGB16UtoPlanar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an unsigned 16-bit-per-channel, 4-channel interleaved buffer into four unsigned 16-bit planar buffers.

### Deinterleaving RGB565 16-bit three-channel interleaved buffers

func vImageConvert_RGB565toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an RGB565 3-channel interleaved buffer into three 8-bit planar buffers.

### Deinterleaving ARGB1555 16-bit four-channel interleaved buffers

func vImageConvert_ARGB1555toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an ARGB1555 4-channel interleaved buffer into four 8-bit planar buffers.

## See Also

### Converting between interleaved and planar formats

Functions that interleave integer planar buffers

Combine discrete integer planar buffers into an interleaved buffer.

Functions that interleave noninteger planar buffers

Combine discrete fixed- and floating-point planar buffers into an interleaved buffer.

Functions that deinterleave noninteger interleaved buffers

Separate fixed- and floating-point interleaved buffers into discrete planar buffers.

