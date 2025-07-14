

- Accelerate
-  vImageLookupTable_PlanarFtoPlanar8(\_:\_:\_:\_:) 

Function

# vImageLookupTable_PlanarFtoPlanar8(\_:\_:\_:\_:)

Uses a lookup table to transform a 32-bit planar image to an 8-bit planar image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageLookupTable_PlanarFtoPlanar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ table: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`table`  

A lookup table that contains 4,096 Pixel_8 values.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function maps the source pixels in the range `0...1` to the index values `0...4095`. The per-pixel conversion calculation is equivalent to the following:

```
uint8_t table[4096];
uint32_t index =  (uint32_t) MIN( MAX( input_float_pixel * 4096.0f, 0.0f), 4095.0f);
uint8_t result_pixel = table[ index ];
```

You can use this function with multichannel data by scaling the width of the image to compensate for the additional channels. In this case, all channels use the same lookup table.

This function works in place, provided that `src->data == dest->data` and `src->rowBytes >= dest->rowBytes`. If `src->rowBytes > dest->rowBytes`, pass the kvImageDoNotTile flag.

## See Also

### Transforming planar-to-planar with a lookup table

func vImageTableLookUp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an 8-bit planar image.

func vImageLookupTable_Planar8toPlanar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an unsigned 16-bit planar image.

func vImageLookupTable_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func vImageLookupTable_8to64U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt64>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 64-bit planar image.

func vImageLookupTable_Planar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 16-bit planar image.

func vImageInterpolatedLookupTable_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImagePixelCount, Float, Float, vImage_Flags) -> vImage_Error

Uses an interpolated lookup table to transform a 32-bit planar image.

