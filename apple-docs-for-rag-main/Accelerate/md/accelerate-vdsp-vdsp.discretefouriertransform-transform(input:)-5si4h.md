

- Accelerate
- vDSP
- vDSP.DiscreteFourierTransform
-  transform(input:) 

Instance Method

# transform(input:)

Returns the result of a double-precision discrete Fourier transform.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func transform(input: U) -> [DSPDoubleComplex] where U : AccelerateBuffer, U.Element == DSPDoubleComplex
```

Available when `T` is `DSPDoubleComplex`.

## Parameters 

`input`  

An array of DSPDoubleComplex structures that contains the input.

## Return Value

An array of DSPDoubleComplex structures.

## See Also

### Performing Interleaved Discrete Fourier Transforms

func transform&lt;U>(input: U) -> [DSPComplex]

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U, V>(input: U, output: inout V)

Computes a single-precision discrete Fourier transform.

func transform&lt;U, V>(input: U, output: inout V)

Computes a double-precision discrete Fourier transform.

