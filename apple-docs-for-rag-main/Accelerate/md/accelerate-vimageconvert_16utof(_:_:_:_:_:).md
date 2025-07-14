

- Accelerate
-  vImageConvert_16UToF(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_16UToF(\_:\_:\_:\_:\_:)

Converts an unsigned 16-bit planar buffer to a floating-point 32-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_16UToF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ offset: Float,
    _ scale: Float,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`offset`  

The offset value that the conversion adds to each pixel.

`scale`  

The scale value that the conversion multiplies each pixel by.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
float result = (float) srcPixel * scale + offset
```

## See Also

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_16Uto16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to a floating-point 16-bit planar buffer.

func vImageConvert_16Uto16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to a fixed-point 16-bit planar buffer.

