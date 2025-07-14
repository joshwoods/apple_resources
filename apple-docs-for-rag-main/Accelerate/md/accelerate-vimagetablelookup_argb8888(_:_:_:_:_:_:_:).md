

- Accelerate
-  vImageTableLookUp_ARGB8888(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageTableLookUp_ARGB8888(\_:\_:\_:\_:\_:\_:\_:)

Uses a lookup table to transform an interleaved, four-channel 8-bit planar image to an interleaved, four-channel 8-bit planar image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageTableLookUp_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ alphaTable: UnsafePointer!,
    _ redTable: UnsafePointer!,
    _ greenTable: UnsafePointer!,
    _ blueTable: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`alphaTable`  

A lookup table for the alpha channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the alpha channel unchanged to the destination buffer.

`redTable`  

A lookup table for the red channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the alpha channel unchanged to the destination buffer.

`greenTable`  

A lookup table for the green channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the alpha channel unchanged to the destination buffer.

`blueTable`  

A lookup table for the blue channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the alpha channel unchanged to the destination buffer.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

