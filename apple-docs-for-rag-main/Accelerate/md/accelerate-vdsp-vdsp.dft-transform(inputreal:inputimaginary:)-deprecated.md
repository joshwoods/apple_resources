

- Accelerate
- vDSP
- vDSP.DFT
-  transform(inputReal:inputImaginary:) Deprecated

Instance Method

# transform(inputReal:inputImaginary:)

Returns a discrete Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func transform(
    inputReal: U,
    inputImaginary: U
) -> (real: [T], imaginary: [T]) where T == U.Element, U : AccelerateBuffer
```

Deprecated

Use `vDSP.DiscreteFourierTransform`.

## See Also

### Instance Methods

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes an out-of-place discrete Fourier transform.

Deprecated

