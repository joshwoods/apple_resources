

- Accelerate
-  vImageConvert_ARGB8888To420Yp8_CbCr8(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB8888To420Yp8_CbCr8(\_:\_:\_:\_:\_:\_:)

Converts an 8-bit-per-channel, 4-channel ARGB buffer to a planar Yp buffer and a 2-channel CbCr buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_ARGB8888To420Yp8_CbCr8(
    _ src: UnsafePointer,
    _ destYp: UnsafePointer,
    _ destCbCr: UnsafePointer,
    _ info: UnsafePointer,
    _ permuteMap: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`destYp`  

A pointer to the Yp destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the Yp destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`destCbCr`  

A pointer to the CbCr destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the CbCr destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`info`  

A vImage_ARGBToYpCbCr structure that describes the conversion matrix, the range of the input and output pixels from the matrix, and clamping information.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## See Also

### Converting to 4:2:0

func vImageConvert_ARGB8888To420Yp8_Cb8_Cr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_ARGBToYpCbCr>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel ARGB buffer to planar Yp, Cb, and Cr buffers.

