

- Accelerate
-  vImageConvert_444CrYpCb8ToARGB8888(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_444CrYpCb8ToARGB8888(\_:\_:\_:\_:\_:\_:)

Converts an 8-bit-per-channel 4:4:4 CrYpCb buffer to an 8-bit-per-channel, 4-channel ARGB buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_444CrYpCb8ToARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ info: UnsafePointer,
    _ permuteMap: UnsafePointer!,
    _ alpha: UInt8,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`info`  

A vImage_YpCbCrToARGB structure that describes the conversion matrix, the range of the input and output pixels from the matrix, and clamping information.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`alpha`  

The constant destination alpha value.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## See Also

### Converting from 4:4:4

func vImageConvert_444AYpCbCr8ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel 4:4:4 YpCbCr buffer to an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_444CbYpCrA8ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel 4:4:4 CbYpCrA buffer to an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_444CrYpCb10ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, UInt8, vImage_Flags) -> vImage_Error

Converts an 10-bit-per-channel 4:4:4 CrYpCb buffer to an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_444CrYpCb10ToARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, Pixel_16Q12, vImage_Flags) -> vImage_Error

Converts an 10-bit-per-channel 4:4:4 CrYpCb buffer to a fixed-point 16-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_444AYpCbCr16ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 16-bit-per-channel 4:4:4 YpCbCr buffer to an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_444AYpCbCr16ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_YpCbCrToARGB>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an 10-bit-per-channel 4:4:4 CrYpCb buffer to an unsigned 16-bit-per-channel, 4-channel ARGB buffer.

