

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyPolynomial(coefficientSegments:boundaries:destination:) 

Instance Method

# applyPolynomial(coefficientSegments:boundaries:destination:)

Applies a set of piecewise polynomials to a 2-channel, 32-bit interleaved buffer and writes the result to a 2-channel, 8-bit interleaved buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyPolynomial(
    coefficientSegments: [[Float]],
    boundaries: [Float],
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.InterleavedFx2`.

## Parameters 

`coefficientSegments`  

An array that contains the polynomial coefficient array. Each polynomial must be of the same order.

`boundaries`  

An array of boundary values, in increasing order, that separates adjacent ranges of pixel values. `boundaries` must contain `coefficientSegments.count + 1` elements.

`destination`  

The destination pixel buffer.

## Discussion

The following code shows an example of applying three polynomials to a vImage.InterleavedFx2 buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [0.25, 0.5, 0.75, 1.0],
    size: vImage.Size(width: 2, height: 1))

let dest = vImage.PixelBuffer(
    size: src.size)

let factor = Float(255)
src.applyPolynomial(coefficientSegments: [ [1 * factor, 0, 0],
                                           [0, 1 * factor, 0],
                                           [0, 0, 1 * factor] ],
                    boundaries: [0, 1/3, 2/3, 1] as [Float],
                    destination: dest)

// Prints:
//  255     ≅ factor * 0.25⁰

//  127     ≅ factor * 0.5¹

//  143     ≅ factor * 0.75²
//  255     ≅ factor * 1.0²
print(dest.array)
```

## See Also

### Related Documentation

Applying tone curve adjustments to images

Use the vImage library’s polynomial transform to apply tone curve adjustments to images.

### Appying polynomial (32-bit source, 8-bit destination)

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Applies a set of piecewise polynomials to a 32-bit planar buffer and writes the result to an 8-bit planar buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a set of piecewise polynomials to a 3-channel, 32-bit interleaved buffer and writes the result to a 3-channel, 8-bit interleaved buffer.

func applyPolynomial(coefficientSegments: [[Float]], boundaries: [Float], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a set of piecewise polynomials to a 4-channel, 32-bit interleaved buffer and writes the result to a 4-channel, 8-bit interleaved buffer.

