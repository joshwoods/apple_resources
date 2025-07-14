

- Accelerate
-  vImageConvert_ARGB16UToXRGB2101010(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB16UToXRGB2101010(\_:\_:\_:\_:\_:\_:)

Converts an unsigned 16-bit-per-channel, 4-channel interleaved buffer to an XRGB2101010 32-bit, 4-channel buffer with permutation.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func vImageConvert_ARGB16UToXRGB2101010(
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

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`RGB101010RangeMin`  

The minimum pixel value for the destination image.

`RGB101010RangeMax`  

The maximum pixel value for the destination image.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
 uint16_t *srcPixel = src.data;
 R16 = srcPixel[permuteMap[1]];
 G16 = srcPixel[permuteMap[2]];
 B16 = srcPixel[permuteMap[3]];
 srcPixel += 4;

 int32_t R10, G10, B10;
 int32_t range10 = RGB101010RangeMax - RGB101010RangeMin;
 R10 = ((R16 * range10 + (USHRT_MAX >> 1)) / USHRT_MAX) + RGB101010RangeMin;
 G10 = ((G16 * range10 + (USHRT_MAX >> 1)) / USHRT_MAX) + RGB101010RangeMin;
 B10 = ((B16 * range10 + (USHRT_MAX >> 1)) / USHRT_MAX) + RGB101010RangeMin;

 uint32_t *destPixel = dest.data;
 destPixel[0] = (R10 

## See Also

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_ARGB16UToRGBA1010102(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel interleaved buffer to an RGBA1010102 32-bit, 4-channel buffer with permutation.

func vImageConvert_ARGB16UToARGB2101010(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit-per-channel, 4-channel interleaved buffer to an ARGB2101010 32-bit, 4-channel buffer with permutation.

