

- Accelerate
-  vImageConvert_16SToF(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_16SToF(\_:\_:\_:\_:\_:)

Converts a signed 16-bit planar buffer to a floating-point 32-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_16SToF(
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
 float result = (float) srcPixel * scale + offset;
```

