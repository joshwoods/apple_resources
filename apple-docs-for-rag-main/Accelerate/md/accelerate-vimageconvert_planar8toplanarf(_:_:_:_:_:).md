

- Accelerate
-  vImageConvert_Planar8toPlanarF(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar8toPlanarF(\_:\_:\_:\_:\_:)

Converts an 8-bit planar buffer to a floating-point 32-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar8toPlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ maxFloat: Pixel_F,
    _ minFloat: Pixel_F,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`maxFloat`  

The maximum pixel value for the destination image.

`minFloat`  

The minimum pixel value for the destination image.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
 float result = (maxFloat - minFloat) * (float) srcPixel / 255.0  + minFloat
```

The two buffers must have the same number of rows and the same number of columns.

## See Also

### Converting from 8-bit buffers

func vImageConvert_8to16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a fixed-point 16-bit planar buffer.

func vImageConvert_Planar8toPlanar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a floating-point 16-bit planar buffer.

