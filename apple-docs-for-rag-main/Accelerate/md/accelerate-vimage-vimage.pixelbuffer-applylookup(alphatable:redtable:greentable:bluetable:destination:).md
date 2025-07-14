

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyLookup(alphaTable:redTable:greenTable:blueTable:destination:) 

Instance Method

# applyLookup(alphaTable:redTable:greenTable:blueTable:destination:)

Applies a set of four lookup tables to transform an interleaved, four-channel 8-bit image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func applyLookup(
    alphaTable: [Pixel_8]?,
    redTable: [Pixel_8]?,
    greenTable: [Pixel_8]?,
    blueTable: [Pixel_8]?,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`alphaTable`  

A lookup table for the alpha channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the alpha channel unchanged to the destination buffer.

`redTable`  

A lookup table for the red channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the red channel unchanged to the destination buffer.

`greenTable`  

A lookup table for the green channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the green channel unchanged to the destination buffer.

`blueTable`  

A lookup table for the blue channel that contains 256 Pixel_8 values. Pass `nil` to specify that the function copies the blue channel unchanged to the destination buffer.

`destination`  

The destination pixel buffer.

## Discussion

Use this function to apply individual lookup tables to each channel in an interleaved, four-channel image. Adjust the order of the tables for images that don’t use ARGB channel ordering. For example, use the `blueTable` parameter for the alpha lookup table to transform an RGBA image.

The following code creates a simple lookup table that transforms a vImage.Interleaved8x4 pixel buffer into its negative. For example, when an input pixel has the value `255, 255, 255, 255`, the output pixel has the value `0, 0, 0, 0`. Conversely, when an input pixel has the value `0, 0, 0, 0`, the output pixel has the value `255, 255, 255, 255`.

```

let lookup: [Pixel_8] = (0 ..

The images below show an example source image on the left and the negative result on the right.

## See Also

### Transforming with a lookup table

func applyLookup([Pixel_8], destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a lookup table to transform an 8-bit planar image.

func applyLookup([Pixel_F], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func applyLookup([Pixel_16U], destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Applies a lookup table to transform an 8-bit planar image to a 16-bit planar image.

func applyLookup([Pixel_8888], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a lookup table to transform an 8-bit planar image to an 8-bit-per-channel, three-channel interleaved image.

func applyLookup([Pixel_FFFF], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, three-channel interleaved image.

