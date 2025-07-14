

- Accelerate
-  vImageHistogramCalculation_Planar8(\_:\_:\_:) 

Function

# vImageHistogramCalculation_Planar8(\_:\_:\_:)

Calculates the histogram of an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageHistogramCalculation_Planar8(
    _ src: UnsafePointer,
    _ histogram: UnsafeMutablePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`histogram`  

The collection that contains 256 elements that receives the histogram data.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The following code populates the `histogram` array with the histogram of the specified vImage_Buffer structure.

```
var histogram = [vImagePixelCount](repeating: 0, count: 256)

// `buffer` is a `vImage_Buffer` structure.
_ = vImageHistogramCalculation_Planar8(&buffer,
                                       &histogram,
                                       vImage_Flags(kvImageNoFlags))
```

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

### Calculating a histogram

func vImageHistogramCalculation_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;vImagePixelCount>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Calculates the histogram of a 32-bit planar buffer.

func vImageHistogramCalculation_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;vImagePixelCount>?>, vImage_Flags) -> vImage_Error

Calculates the histogram of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageHistogramCalculation_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;vImagePixelCount>?>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Calculates the histogram of a 32-bit-per-channel, 4-channel interleaved buffer.

