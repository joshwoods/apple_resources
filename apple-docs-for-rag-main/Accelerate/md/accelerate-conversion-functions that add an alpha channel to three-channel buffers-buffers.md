

- Accelerate
- Conversion
-  Functions that add an alpha channel to three-channel buffers 

API Collection

# Functions that add an alpha channel to three-channel buffers

Add a constant alpha value or planar alpha buffer to an RGB image.

## Topics

### Conversion from 8-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB888toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce an ARGB result.

vImageConvert_BGR888toBGRA8888

Combines an 8-bit-per-channel, 3-channel BGR buffer and either an 8-bit alpha buffer or constant alpha value to produce a BGRA result.

func vImageConvert_RGB888toBGRA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce a BGRA result.

vImageConvert_BGR888toRGBA8888

Combines an 8-bit-per-channel, 3-channel BGR buffer and either an 8-bit alpha buffer or constant alpha value to produce an RGBA result.

func vImageConvert_RGB888toRGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce an RGBA result.

### Conversion from unsigned 16-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB16UToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 3-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer using permutation.

func vImageConvert_RGB16UtoARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce an ARGB result.

func vImageConvert_RGB16UtoBGRA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce a BGRA result.

func vImageConvert_RGB16UtoRGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce an RGBA result.

### Conversion from RGB565 16-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB565toARGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_RGB565toBGRA8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel BGRA buffer.

func vImageConvert_RGB565toRGBA8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel RGBA buffer.

func vImageConvert_RGB565toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel ARGB1555 buffer.

func vImageConvert_RGB565toRGBA5551(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel RGBA5551 buffer.

### Conversion from 32-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGBFFFtoARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_F, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines a floating-point 32-bit-per-channel, 3-channel RGB buffer and either an 32-bit alpha buffer or constant alpha value to produce an ARGB result.

func vImageConvert_RGBFFFtoBGRAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_F, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines a floating-point 32-bit-per-channel, 3-channel RGB buffer and either an 32-bit alpha buffer or constant alpha value to produce a BGRA result.

func vImageConvert_RGBFFFtoRGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_F, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines a floating-point 32-bit-per-channel, 3-channel RGB buffer and either an 32-bit alpha buffer or constant alpha value to produce an RGBA result.

## See Also

### Adding and removing alpha channels

Functions that remove an alpha channel from four-channel buffers

Remove the alpha channel from an RGBA or ARGB buffer.

