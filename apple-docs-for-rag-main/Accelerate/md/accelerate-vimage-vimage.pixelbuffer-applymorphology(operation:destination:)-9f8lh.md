

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyMorphology(operation:destination:) 

Instance Method

# applyMorphology(operation:destination:)

Applies a morphology operation to a 32-bit planar pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyMorphology(
    operation: vImage.MorphologyOperation,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`operation`  

An enumeration that specifies the morphology operation.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Adding a bokeh effect to images

Simulate a bokeh effect by applying dilation.

### Morphology

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to an 8-bit planar pixel buffer.

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_8>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func applyMorphology(operation: vImage.MorphologyOperation&lt;Pixel_F>, destination: vImage.PixelBuffer&lt;Format>)

Applies a morphology operation to a 32-bit-per-channel, 4-channel interleaved pixel buffer.

enum MorphologyOperation

Describes which morphology operation to perform.

typealias StructuringElement

A 2D matrix that represents a morphology kernel.

