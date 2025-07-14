

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyPolynomial(coefficientSegments:boundaries:destination:) 

Instance Method

# applyPolynomial(coefficientSegments:boundaries:destination:)

Applies a set of piecewise polynomials to a 2-channel, 8-bit interleaved buffer and writes the result to a 2-channel, 32-bit interleaved buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyPolynomial(
    coefficientSegments: [[Float]],
    boundaries: [Float],
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x2`.

## Parameters 

`coefficientSegments`  

An array that contains the polynomial coefficient array. Each polynomial must be of the same order.

`boundaries`  

An array of boundary values, in increasing order, that separates adjacent ranges of pixel values. `boundaries` must contain `coefficientSegments.count + 1` elements.

`destination`  

The destination pixel buffer.

## Discussion

The following code shows an example of applying three polynomials to an vImage.Interleaved8x2 buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [64, 128, 192, 255],
    size: vImage.Size(width: 2, height: 1))

let dest = vImage.PixelBuffer(
    size: src.size)

src.applyPolynomial(coefficientSegments: [ [1, 0, 0],
                                           [0, 1, 0],
                                           [0, 0, 1] ],
                    boundaries: [0, 1/3, 2/3, 1] as [Float],
                    destination: dest)

// Prints:
//  1.0         ≅ 1 * (64 / 255)⁰

//  0.5019608   ≅ 1 * (128 / 255)¹

//  0.56692046  ≅ 1 * (192 / 255)²
//  1.0         ≅ 1 * (255 / 255)²
print(dest.array)
```

## See Also

### Related Documentation

Applying tone curve adjustments to images

Use the vImage library’s polynomial transform to apply tone curve adjustments to images.

### Appying polynomial (8-bit source, 32-bit destination)

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a set of piecewise polynomials to an 8-bit planar buffer and writes the result to a 32-bit planar buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a set of piecewise polynomials to a 3-channel, 8-bit interleaved buffer and writes the result to a 3-channel, 32-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Applies a set of piecewise polynomials to a 4-channel, 8-bit interleaved buffer and writes the result to a 4-channel, 32-bit interleaved buffer.

