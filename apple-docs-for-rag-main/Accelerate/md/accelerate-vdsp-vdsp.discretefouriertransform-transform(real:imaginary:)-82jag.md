

- Accelerate
- vDSP
- vDSP.DiscreteFourierTransform
-  transform(real:imaginary:) 

Instance Method

# transform(real:imaginary:)

Returns the result of a double-precision discrete Fourier transform.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func transform(
    real: U,
    imaginary: U
) -> (real: [Double], imaginary: [Double]) where U : AccelerateBuffer, U.Element == Double
```

Available when `T` is `Double`.

## Parameters 

`real`  

An array that contains the real parts of the input.

`imaginary`  

An array that contains the imaginary parts of the input.

## Return Value

A tuple of two arrays that represents the real and imaginary parts of the output.

## See Also

### Performing Split-Complex Discrete Fourier Transforms

func transform&lt;U>(real: U, imaginary: U) -> (real: [Float], imaginary: [Float])

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes a single-precision discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes a double-precision discrete Fourier transform.

