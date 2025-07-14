

- Accelerate
-  vImageLookupTable_8to64U(\_:\_:\_:\_:) 

Function

# vImageLookupTable_8to64U(\_:\_:\_:\_:)

Uses a lookup table to transform an 8-bit planar image to a 64-bit planar image.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageLookupTable_8to64U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ LUT: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`LUT`  

A lookup table that contains 256 uint64_t values.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

For each pixel, this function uses the 8-bit value from the source image as an index to the 64-bit value from the table. The per-pixel conversion calculation is equivalent to the following:

```
uint64_t table[256];
uint64_t result_pixel = table[ input_8_bit_pixel ];
```

You can use this function with multichannel data by scaling the width of the image to compensate for the additional channels. In this case, all channels use the same lookup table.

This function doesn’t work in place.

## See Also

### Transforming planar-to-planar with a lookup table

func vImageTableLookUp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an 8-bit planar image.

func vImageLookupTable_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 32-bit planar image to an 8-bit planar image.

func vImageLookupTable_Planar8toPlanar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an unsigned 16-bit planar image.

func vImageLookupTable_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func vImageLookupTable_Planar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 16-bit planar image.

func vImageInterpolatedLookupTable_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImagePixelCount, Float, Float, vImage_Flags) -> vImage_Error

Uses an interpolated lookup table to transform a 32-bit planar image.

