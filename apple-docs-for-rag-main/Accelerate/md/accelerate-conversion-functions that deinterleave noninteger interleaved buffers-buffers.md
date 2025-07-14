

- Accelerate
- Conversion
-  Functions that deinterleave noninteger interleaved buffers 

API Collection

# Functions that deinterleave noninteger interleaved buffers

Separate fixed- and floating-point interleaved buffers into discrete planar buffers.

## Topics

### Deinterleaving 32-bit interleaved buffers

func vImageConvert_ChunkyToPlanarF(UnsafeMutablePointer&lt;UnsafeRawPointer?>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UInt32, Int, vImagePixelCount, vImagePixelCount, Int, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel interleaved buffer with an arbitrary number of channels into the corresponding number of 32-bit planar buffers.

### Deinterleaving 32-bit three-channel interleaved buffers

func vImageConvert_RGBFFFtoPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 3-channel interleaved buffer into three floating-point 32-bit planar buffers.

### Deinterleaving 32-bit four-channel interleaved buffers

func vImageConvert_ARGBFFFFtoPlanar8(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into four 8-bit planar buffers.

func vImageConvert_BGRXFFFFToPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into three floating-point 32-bit planar buffers and discards the last channel.

func vImageConvert_XRGBFFFFToPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into three floating-point 32-bit planar buffers and discards the first channel.

func vImageConvert_ARGBFFFFtoPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into four floating-point 38-bit planar buffers.

## See Also

### Converting between interleaved and planar formats

Functions that interleave integer planar buffers

Combine discrete integer planar buffers into an interleaved buffer.

Functions that interleave noninteger planar buffers

Combine discrete fixed- and floating-point planar buffers into an interleaved buffer.

Functions that deinterleave integer interleaved buffers

Separate integer interleaved buffers into discrete planar buffers.

