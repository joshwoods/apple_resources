

- Accelerate
-  vImageConvert_ARGB16UtoPlanar16U(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB16UtoPlanar16U(\_:\_:\_:\_:\_:\_:)

Deinterleaves an unsigned 16-bit-per-channel, 4-channel interleaved buffer into four unsigned 16-bit planar buffers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_ARGB16UtoPlanar16U(
    _ argbSrc: UnsafePointer,
    _ aDest: UnsafePointer,
    _ rDest: UnsafePointer,
    _ gDest: UnsafePointer,
    _ bDest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`argbSrc`  

The source vImage buffer.

`aDest`  

A pointer to the alpha destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the alpha destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`rDest`  

A pointer to the red destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the red destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`gDest`  

A pointer to the green destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the green destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`bDest`  

A pointer to the blue destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the blue destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The source and destination buffers must have the same height and width.

