

- Accelerate
-  vImageVerticalShear_CbCr16S(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageVerticalShear_CbCr16S(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func vImageVerticalShear_CbCr16S(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ yTranslate: Float,
    _ shearSlope: Float,
    _ filter: ResamplingFilter!,
    _ backColor: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## See Also

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

