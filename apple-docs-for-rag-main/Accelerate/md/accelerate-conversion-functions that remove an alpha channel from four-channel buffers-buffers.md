

- Accelerate
- Conversion
-  Functions that remove an alpha channel from four-channel buffers 

API Collection

# Functions that remove an alpha channel from four-channel buffers

Remove the alpha channel from an RGBA or ARGB buffer.

## Topics

### Conversion from 8-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_RGBA8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_BGRA8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel BGRA buffer to produce an 8-bit-per-channel RGB result.

vImageConvert_BGRA8888toBGR888

Removes the alpha channel from an 8-bit-per-channel BGRA buffer to produce an 8-bit-per-channel BGR result.

vImageConvert_RGBA8888toBGR888

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an 8-bit-per-channel BGR result.

func vImageConvert_ARGB8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an RGB565 result.

func vImageConvert_ARGB8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_BGRA8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an RGB565 result.

func vImageConvert_BGRA8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel BGRA buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_RGBA8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_RGBA8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an RGB565 result.

func vImageConvert_ARGB8888ToRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an unsigned 16-bit-per-channel RGB result.

### Conversion from unsigned 16-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an unsigned 16-bit-per-channel ARGB buffer to produce an unsigned 16-bit-per-channel RGB result.

func vImageConvert_BGRA16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an unsigned 16-bit-per-channel BGRA buffer to produce an unsigned 16-bit-per-channel RGB result.

func vImageConvert_RGBA16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an unsigned 16-bit-per-channel RGBA buffer to produce an unsigned 16-bit-per-channel RGB result.

### Conversion from ARGB1555 16-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB1555toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an ARGB1555 buffer to produce an RGB565 result.

func vImageConvert_RGBA5551toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an RGBA5551 buffer to produce an RGB565 result.

### Conversion from 32-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGBFFFFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Removes the alpha channel from a floating-point 32-bit-per-channel ARGB buffer to produce a floating-point 32-bit-per-channel RGB result.

func vImageConvert_BGRAFFFFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Removes the alpha channel from a floating-point 32-bit-per-channel BGRA buffer to produce a floating-point 32-bit-per-channel RGB result.

func vImageConvert_RGBAFFFFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Removes the alpha channel from a floating-point 32-bit-per-channel RGBA buffer to produce a floating-point 32-bit-per-channel RGB result.

## See Also

### Adding and removing alpha channels

Functions that add an alpha channel to three-channel buffers

Add a constant alpha value or planar alpha buffer to an RGB image.

