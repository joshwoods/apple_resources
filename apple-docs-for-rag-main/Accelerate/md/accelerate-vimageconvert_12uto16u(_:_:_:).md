

- Accelerate
-  vImageConvert_12UTo16U(\_:\_:\_:) 

Function

# vImageConvert_12UTo16U(\_:\_:\_:)

Converts an unsigned 12-bit planar buffer to an unsigned 16-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_12UTo16U(
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
 uint8_t *srcRow = srcData;
 uint16_t *destRow = destData;

 // Load two 12-bit values.
 t0 = (srcRow[0] >= 12;

 //Convert and store.
 destRow[0] = (t0 * 65535U + (t0 > 12;
 destRow[1] = (t1 * 65535U + (t1 > 12;
 destRow += 2;
```

