

- Accelerate
- Image shearing
-  Single-precision vertical shearing 

API Collection

# Single-precision vertical shearing

Apply single-precision vertical shearing to images.

## Topics

### Shearing 8-bit-per-channel buffers

func vImageVerticalShear_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_8, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an 8-bit planar image.

func vImageVerticalShear_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an 8-bit-per-channel, 2-channel interleaved image.

func vImageVerticalShear_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an 8-bit-per-channel, 4-channel interleaved image.

### Shearing 10-bit-per-channel buffers

func vImageVerticalShear_XRGB2101010W(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_32U, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a 2-bit alpha, 10-bit RGB interleaved image.

### Shearing 16-bit-per-channel buffers

func vImageVerticalShear_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_16U, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an unsigned 16-bit planar image.

func vImageVerticalShear_Planar16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_16S, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a signed 16-bit planar image.

func vImageVerticalShear_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_16F, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a floating-point 16-bit planar image.

func vImageVerticalShear_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an unsigned 16-bit-per-channel, 2-channel interleaved image.

func vImageVerticalShear_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a floating-point 16-bit-per-channel, 2-channel interleaved image.

func vImageVerticalShear_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageVerticalShear_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageVerticalShear_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a floating-point 16-bit-per-channel, 4-channel interleaved image.

### Shearing 32-bit-per-channel buffers

func vImageVerticalShear_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, Pixel_F, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a 32-bit planar image.

func vImageVerticalShear_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Performs a single-precision vertical shear on a region of interest within a 32-bit-per-channel, 4-channel interleaved image.

## See Also

### Shearing an image vertically

Double-precision vertical shearing

Apply double-precision vertical shearing to images.

