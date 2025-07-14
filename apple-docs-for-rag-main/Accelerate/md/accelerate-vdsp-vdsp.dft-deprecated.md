

- Accelerate
- vDSP
-  vDSP.DFT Deprecated

Class

# vDSP.DFT

A single- and double-precision discrete Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+watchOS 6.0+visionOS

``` source
class DFT where T : vDSP_FloatingPointDiscreteFourierTransformable
```

Deprecated

Use vDSP.DiscreteFourierTransform instead.

## Topics

### Initializers

init?(previous: vDSP.DFT&lt;T>?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType, ofType: T.Type)

Initializes a new discrete Fourier transform instance.

### Instance Methods

func transform&lt;U>(inputReal: U, inputImaginary: U) -> (real: [T], imaginary: [T])

Returns a discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes an out-of-place discrete Fourier transform.

## See Also

### Objects that simplify discrete Fourier transforms

class DiscreteFourierTransform

An object that provides forward and inverse discrete Fourier transforms on single- or double-precision collections of interleaved or split-complex data.

enum DFTTransformType

Discrete Fourier transform types.

