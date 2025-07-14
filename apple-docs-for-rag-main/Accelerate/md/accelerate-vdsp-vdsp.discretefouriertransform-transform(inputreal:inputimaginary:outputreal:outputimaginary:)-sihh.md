

- Accelerate
- vDSP
- vDSP.DiscreteFourierTransform
-  transform(inputReal:inputImaginary:outputReal:outputImaginary:) 

Instance Method

# transform(inputReal:inputImaginary:outputReal:outputImaginary:)

Computes a single-precision discrete Fourier transform.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func transform(
    inputReal: U,
    inputImaginary: U,
    outputReal: inout V,
    outputImaginary: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

Available when `T` is `Float`.

## Parameters 

`inputReal`  

An array that contains the real parts of the input.

`inputImaginary`  

An array that contains the imaginary parts of the input.

`outputReal`  

An array that contains the real parts of the output.

`outputImaginary`  

An array that contains the imaginary parts of the output.

## See Also

### Performing Split-Complex Discrete Fourier Transforms

func transform&lt;U>(real: U, imaginary: U) -> (real: [Float], imaginary: [Float])

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U>(real: U, imaginary: U) -> (real: [Double], imaginary: [Double])

Returns the result of a double-precision discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes a double-precision discrete Fourier transform.

