

- Accelerate
-  vImageContrastStretch_Planar8(\_:\_:\_:) 

Function

# vImageContrastStretch_Planar8(\_:\_:\_:)

Performs contrast stretching on an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageContrastStretch_Planar8(
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

Contrast stretching evenly distributes a histogram’s pixel values across the full range of available pixel values. This technique is ideal for enhancing the contrast of an image with pixel values concentrated in one area of the intensity spectrum.

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

### Performing contrast stretching

func vImageContrastStretch_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs contrast stretching on a 32-bit planar buffer.

func vImageContrastStretch_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs contrast stretching on an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageContrastStretch_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UInt32, Pixel_F, Pixel_F, vImage_Flags) -> vImage_Error

Performs contrast stretching on a 32-bit-per-channel, 4-channel interleaved buffer.

