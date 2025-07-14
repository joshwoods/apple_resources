

- Accelerate
- Image shearing
-  Double-precision vertical shearing 

API Collection

# Double-precision vertical shearing

Apply double-precision vertical shearing to images.

## Topics

### Shearing 8-bit-per-channel buffers

func vImageVerticalShearD_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, Pixel_8, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within an 8-bit planar image.

func vImageVerticalShearD_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within an 8-bit-per-channel, 4-channel interleaved image.

### Shearing 16-bit-per-channel buffers

func vImageVerticalShearD_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, Pixel_16F, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a floating-point 16-bit planar image.

func vImageVerticalShearD_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a floating-point 16-bit-per-channel, 2-channel interleaved image.

func vImageVerticalShearD_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageVerticalShearD_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageVerticalShearD_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a floating-point 16-bit-per-channel, 4-channel interleaved image.

func vImageVerticalShearD_CbCr16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

func vImageVerticalShearD_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

func vImageVerticalShear_CbCr16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Float, Float, ResamplingFilter!, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

### Shearing 32-bit-per-channel buffers

func vImageVerticalShearD_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, Pixel_F, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a 32-bit planar image.

func vImageVerticalShearD_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, Double, Double, ResamplingFilter!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Performs a double-precision vertical shear on a region of interest within a 32-bit-per-channel, 4-channel interleaved image.

## See Also

### Shearing an image vertically

Single-precision vertical shearing

Apply single-precision vertical shearing to images.

