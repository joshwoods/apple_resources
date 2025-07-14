

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyLookup(\_:destination:) 

Instance Method

# applyLookup(\_:destination:)

Applies a lookup table to transform an 8-bit planar image to an 8-bit-per-channel, three-channel interleaved image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func applyLookup(
    _ lookupTable: [Pixel_8888],
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Planar8`.

## Parameters 

`lookupTable`  

A lookup table that contains 256 Pixel_8888 ARGB values. The function discards the alpha component.

`destination`  

The destination pixel buffer.

## Discussion

You can use this function to create pseudo-color images by transforming a grayscale image to an RGB image.

The following code creates a simple lookup table with a high red response for low values, a high green response for middle values, and a high blue response for large values:

```
let window = vDSP.window(ofType: Float.self,
                         usingSequence: .blackman,
                         count: 256,
                         isHalfWindow: false)

let lookup: [Pixel_8888] = (0 ..

The graph below visualizes the values in the lookup table:

Use the following code to apply the lookup table to a vImage.Planar8 source buffer with a vImage.Interleaved8x3 destination buffer:

```
let destinationBuffer = vImage.PixelBuffer (
    size: sourceBuffer.size,
    pixelFormat: vImage.Interleaved8x3.self)

sourceBuffer.applyLookup(lookup, destination: destinationBuffer)
```

The images below show an example grayscale source image on the left and the pseudo-color result on the right. The operation converts dark areas in the source to red in the destination, and light areas in the source to blue in the destination.

## See Also

### Transforming with a lookup table

func applyLookup([Pixel_8], destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a lookup table to transform an 8-bit planar image.

func applyLookup([Pixel_F], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func applyLookup([Pixel_16U], destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Applies a lookup table to transform an 8-bit planar image to a 16-bit planar image.

func applyLookup([Pixel_FFFF], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, three-channel interleaved image.

func applyLookup(alphaTable: [Pixel_8]?, redTable: [Pixel_8]?, greenTable: [Pixel_8]?, blueTable: [Pixel_8]?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a set of four lookup tables to transform an interleaved, four-channel 8-bit image.

