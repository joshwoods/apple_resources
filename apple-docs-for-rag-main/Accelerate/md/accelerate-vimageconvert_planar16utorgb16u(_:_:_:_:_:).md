

- Accelerate
-  vImageConvert_Planar16UtoRGB16U(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar16UtoRGB16U(\_:\_:\_:\_:\_:)

Interleaves three unsigned 16-bit planar buffers into an unsigned 16-bit-per-channel, 3-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar16UtoRGB16U(
    _ rSrc: UnsafePointer,
    _ gSrc: UnsafePointer,
    _ bSrc: UnsafePointer,
    _ rgbDest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`rSrc`  

The source vImage buffer that contains the red channel.

`gSrc`  

The source vImage buffer that contains the green channel.

`bSrc`  

The source vImage buffer that contains the blue channel.

`rgbDest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The source and destination buffers must have the same height and width.

