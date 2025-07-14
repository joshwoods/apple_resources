

- Accelerate
- vDSP
- vDSP.DiscreteFourierTransform
-  transform(input:output:) 

Instance Method

# transform(input:output:)

Computes a double-precision discrete Fourier transform.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func transform(
    input: U,
    output: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == DSPDoubleComplex, V.Element == DSPDoubleComplex
```

Available when `T` is `DSPDoubleComplex`.

## Parameters 

`input`  

An array of DSPDoubleComplex structures that contains the input.

`output`  

An array of DSPDoubleComplex structures that contains the output.

## See Also

### Performing Interleaved Discrete Fourier Transforms

func transform&lt;U>(input: U) -> [DSPComplex]

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U>(input: U) -> [DSPDoubleComplex]

Returns the result of a double-precision discrete Fourier transform.

func transform&lt;U, V>(input: U, output: inout V)

Computes a single-precision discrete Fourier transform.

