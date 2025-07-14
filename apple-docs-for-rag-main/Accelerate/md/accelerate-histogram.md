

- Accelerate
-  Histogram 

API Collection

# Histogram

Calculate or manipulate an image’s histogram.

## Topics

### Performing contrast stretching

func vImageContrastStretch_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs contrast stretching on an 8-bit planar buffer.

func vImageContrastStretch_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs contrast stretching on a 32-bit planar buffer.

func vImageContrastStretch_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs contrast stretching on an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageContrastStretch_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs contrast stretching on a 32-bit-per-channel, 4-channel interleaved buffer.

### Performing ends-in contrast stretching

func vImageEndsInContrastStretch_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Performs ends-in contrast stretching on an 8-bit planar buffer.

func vImageEndsInContrastStretch_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, UInt32, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs ends-in contrast stretching on a 32-bit planar buffer.

func vImageEndsInContrastStretch_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt32>, UnsafePointer&lt;UInt32>, vImage_Flags) -> vImage_Error

Performs ends-in contrast stretching on an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageEndsInContrastStretch_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;UInt32>, UnsafePointer&lt;UInt32>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs ends-in contrast stretching on a 32-bit-per-channel, 4-channel interleaved buffer.

### Equalizing a histogram

func vImageEqualization_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs histogram equalization on an 8-bit planar buffer.

func vImageEqualization_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs histogram equalization on a 32-bit planar buffer.

func vImageEqualization_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs histogram equalization on an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageEqualization_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs histogram equalization on a 32-bit-per-channel, 4-channel interleaved buffer.

### Calculating a histogram

func vImageHistogramCalculation_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;vImagePixelCount>, vImage_Flags) -> vImage_Error

Calculates the histogram of an 8-bit planar buffer.

func vImageHistogramCalculation_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;vImagePixelCount>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Calculates the histogram of a 32-bit planar buffer.

func vImageHistogramCalculation_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;vImagePixelCount>?>, vImage_Flags) -> vImage_Error

Calculates the histogram of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageHistogramCalculation_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;vImagePixelCount>?>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Calculates the histogram of a 32-bit-per-channel, 4-channel interleaved buffer.

### Specifying a histogram

func vImageHistogramSpecification_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImagePixelCount>, vImage_Flags) -> vImage_Error

Specifies the histogram of an 8-bit planar buffer.

func vImageHistogramSpecification_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImagePixelCount>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Specifies the histogram of a 32-bit planar buffer.

func vImageHistogramSpecification_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImagePixelCount>?>, vImage_Flags) -> vImage_Error

Specifies the histogram of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageHistogramSpecification_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UnsafePointer&lt;vImagePixelCount>?>!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Specifes the histogram of a 32-bit-per-channel, 4-channel interleaved buffer.

## See Also

### Color and Tone Adjustment

Adjusting the brightness and contrast of an image

Use a gamma function to apply a linear or exponential curve.

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

Applying tone curve adjustments to images

Use the vImage library’s polynomial transform to apply tone curve adjustments to images.

Adjusting the hue of an image

Convert an image to L\*a\*b\* color space and apply hue adjustment.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

