

- Accelerate
-  vImageConvert_ARGB8888ToARGB16U(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB8888ToARGB16U(\_:\_:\_:\_:\_:\_:)

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel buffer with permutation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_ARGB8888ToARGB16U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ permuteMap: UnsafePointer,
    _ copyMask: UInt8,
    _ backgroundColor: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`copyMask`  

A bitmask that specifies the channel from the background color that the function copies to the destination channel at the corresponding index. The `1000` bit corresponds to the alpha channel, the `0100` bit corresponds to the red channel, the `0010` corresponds to the green channel, and the `0001` bit corresponds to the green channel.

`backgroundColor`  

A 16-bit-per-channel, 4-channel pixel value that replaces the destination pixels based on the copy mask.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
 Pixel_8888 *srcPixel;
 Pixel_16U *destPixel;
 uint8_t result8;
 uint16_t result[4];
 uint8_t mask = 0x8;

 for( int i = 0; i > 1;
 }
 srcPixel += 4;

 destPixel[0] = result[0];
 destPixel[1] = result[1];
 destPixel[2] = result[2];
 destPixel[3] = result[3];
 destPixel += 4;
```

## See Also

### Converting from 8-bit buffers

func vImageConvert_RGB888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 3-channel interleaved buffer to an RGB565 3-channel interleaved buffer using the specified dithering algorithm.

func vImageConvert_ARGB8888toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer.

func vImageConvert_ARGB8888toARGB1555_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_RGBA8888toRGBA5551(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer.

func vImageConvert_RGBA8888toRGBA5551_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer usng the specified dithering algorithm.

