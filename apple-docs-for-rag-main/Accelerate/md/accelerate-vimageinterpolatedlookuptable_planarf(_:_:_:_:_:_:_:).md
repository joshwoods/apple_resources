

- Accelerate
-  vImageInterpolatedLookupTable_PlanarF(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageInterpolatedLookupTable_PlanarF(\_:\_:\_:\_:\_:\_:\_:)

Uses an interpolated lookup table to transform a 32-bit planar image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageInterpolatedLookupTable_PlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ table: UnsafePointer,
    _ tableEntries: vImagePixelCount,
    _ maxFloat: Float,
    _ minFloat: Float,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`table`  

A lookup table that contains Pixel_F values.

`tableEntries`  

The number of values in the lookup table.

`maxFloat`  

A value of type `float`.

`minFloat`  

A value of type `float`.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Provide this function with a lookup table with any number of values, but with a minimum value of `minFloat` and a maximum value of `maxFloat`. The function generates lookup values by linearly interpolating between the supplied values. The per-pixel conversion calculation is equivalent to the following:

```
float clippedPixel = MAX( MIN( src_pixel, maxFloat ), minFloat );    //clip src_pixel to be in range
float fIndex = (float) (tableEntries - 1) * (clippedPixel - minFloat ) / (maxFloat - minFloat);
float fract = fIndex - floor( fIndex );
unsigned long index =  fIndex;
float result = table[ index ] * ( 1.0f - fract ) + table[ index + 1] * fract;
```

The following code shows a lookup table that contains two values, `1` and `0`. The result is that the lookup transformation maps the source values `0...1` to the destination values `1...0`.

```
let lookupTable: [Float] = [1, 0]

let source = vImage.PixelBuffer(
    pixelValues: [0.2, 0.4, 0.6, 0.8],
    size: .init(width: 4, height: 1))

let destination = vImage.PixelBuffer(
    size: source.size)

source.withUnsafePointerToVImageBuffer{ src in
    destination.withUnsafePointerToVImageBuffer { dest in

        _ = vImageInterpolatedLookupTable_PlanarF(
            src,
            dest,
            lookupTable,
            vImagePixelCount(lookupTable.count),
            1, 0,
            vImage_Flags(kvImageNoFlags))
    }
}

// Prints "[0.8, 0.6, 0.4, 0.2]".
print(destination.array)
```

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

func vImageLookupTable_8to64U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt64>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 64-bit planar image.

func vImageLookupTable_Planar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 16-bit planar image.

