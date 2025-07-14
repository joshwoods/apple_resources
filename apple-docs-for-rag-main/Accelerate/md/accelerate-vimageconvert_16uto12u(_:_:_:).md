

- Accelerate
-  vImageConvert_16UTo12U(\_:\_:\_:) 

Function

# vImageConvert_16UTo12U(\_:\_:\_:)

Converts an unsigned 16-bit planar buffer to an unsigned 12-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_16UTo12U(
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

The function uses the following calculation to perform the conversion:

```
 uint16_t *srcRow = srcData;
 uint8_t *destRow = destData;

 // Two 16-bit in 4-bytes.
 t0 = srcRow[0];
 t1 = srcRow[1];
 srcRow += 2;

 t0 = (t0 * 4095 + 32767 + (t0 >> 4)) >> 16;
 t1 = (t1 * 4095 + 32767 + (t1 >> 4)) >> 16;

 t0 > 16;
 destRow[1] = t0 >> 8;
 destRow[2] = t0;
 destRow += 3;
```

## See Also

### Converting from unsigned 16-bit-per-channel buffers

func vImageConvert_16UToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to an 8-bit planar buffer.

func vImageConvert_Planar16UtoPlanar8_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Converts an unsigned 16-bit planar buffer to an 8-bit planar buffer using the specified dithering algorithm.

