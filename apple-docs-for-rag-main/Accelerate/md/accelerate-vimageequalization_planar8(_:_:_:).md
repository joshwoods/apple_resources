

- Accelerate
-  vImageEqualization_Planar8(\_:\_:\_:) 

Function

# vImageEqualization_Planar8(\_:\_:\_:)

Performs histogram equalization on an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageEqualization_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Histogram equalization transforms an image so that its histogram is more uniformly distributed across the entire range of values. The operation stretches dense parts of the histogram, where contrast is low, and condenses sparse parts of the histogram, where contrast is high. A truly uniform histogram is one in which each histogram bin contains the same value, that is, its cumulative histogram is a diagonal line. The vImage histogram equalization functions approximate that truly uniform histogram.

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

### Equalizing a histogram

func vImageEqualization_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs histogram equalization on a 32-bit planar buffer.

func vImageEqualization_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs histogram equalization on an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageEqualization_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs histogram equalization on a 32-bit-per-channel, 4-channel interleaved buffer.

