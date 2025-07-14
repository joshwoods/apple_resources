

- Accelerate
-  vImageConvert_ARGB2101010ToARGB16U(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB2101010ToARGB16U(\_:\_:\_:\_:\_:\_:)

Converts an ARGB2101010 32-bit, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel interleaved buffer with permutation.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func vImageConvert_ARGB2101010ToARGB16U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ RGB101010RangeMin: Int32,
    _ RGB101010RangeMax: Int32,
    _ permuteMap: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to the vImage buffer that references 10-bit RGB interleaved source pixels.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`RGB101010RangeMin`  

The minimum pixel value for the source image range.

`RGB101010RangeMax`  

The maximum pixel value for the source image range.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The `RGB101010RangeMin` and `RGB101010RangeMax` parameters allow you to specify that the function represents source pixel values that are outside of the range `0.0 ... 1.0`. For full-range pixel values, specify `RGB101010RangeMin` and `RGB101010RangeMax` as the following:

```
 RGB101010RangeMin = 0
 RGB101010RangeMax = 1023
```

## See Also

### Converting from XRGB2101010 32-bit buffers

func vImageConvert_ARGB2101010ToARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an ARGB2101010 32-bit, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_XRGB2101010ToARGB8888(UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an XRGB2101010 32-bit, 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer with permutation.

func vImageConvert_XRGB2101010ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UInt16, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an XRGB2101010 32-bit, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel interleaved buffer with permutation.

