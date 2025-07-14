

- Accelerate
-  vImageHistogramSpecification_Planar8(\_:\_:\_:\_:) 

Function

# vImageHistogramSpecification_Planar8(\_:\_:\_:\_:)

Specifies the histogram of an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageHistogramSpecification_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ desired_histogram: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`desired_histogram`  

The histogram that the operation applies to the source buffer.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Use this function to apply a histogram — that you’ve generated using vImageHistogramCalculation_Planar8(_:_:_:) — to another image.

The following code applies a histogram to a planar vImage buffer:

```
// `histogram` is a 256-element array.
histogram.withUnsafeBufferPointer {
    // `buffer` is a `vImage_Buffer` structure.
    _ = vImageHistogramSpecification_Planar8(&buffer, &buffer,
                                             $0.baseAddress!,
                                             vImage_Flags(kvImageNoFlags))
}
```

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

### Specifying a histogram

func vImageHistogramSpecification_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImagePixelCount>, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Specifies the histogram of a 32-bit planar buffer.

func vImageHistogramSpecification_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImagePixelCount>?>, vImage_Flags) -> vImage_Error

Specifies the histogram of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageHistogramSpecification_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UnsafePointer&lt;vImagePixelCount>?>!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Specifes the histogram of a 32-bit-per-channel, 4-channel interleaved buffer.

