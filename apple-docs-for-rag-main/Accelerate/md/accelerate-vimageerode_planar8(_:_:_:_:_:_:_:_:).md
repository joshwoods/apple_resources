

- Accelerate
-  vImageErode_Planar8(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageErode_Planar8(\_:\_:\_:\_:\_:\_:\_:\_:)

Erodes an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageErode_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ kernel: UnsafePointer,
    _ kernel_height: vImagePixelCount,
    _ kernel_width: vImagePixelCount,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernel`  

The kernel data that contains `kernel_height * kernel_width` elements.

`kernel_height`  

The height of the kernel in pixels. This value must be odd.

`kernel_width`  

The width of the kernel in pixels. This value must be odd.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Use the erode operation to enlarge dark structural elements in an image. In the case where the kernel contains all zeros, use the corresponding minimize function instead.

## See Also

### Related Documentation

Adding a bokeh effect to images

Simulate a bokeh effect by applying dilation.

### Eroding an object

func vImageErode_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes a 32-bit planar buffer.

func vImageErode_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;UInt8>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageErode_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes a 32-bit-per-channel, 4-channel interleaved buffer.

