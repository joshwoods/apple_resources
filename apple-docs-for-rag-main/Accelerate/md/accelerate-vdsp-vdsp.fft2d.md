

- Accelerate
- vDSP
-  vDSP.FFT2D 

Class

# vDSP.FFT2D

A 2D single- and double-precision fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
class FFT2D where T : vDSP_FourierTransformable
```

## Topics

### Initializers

init?(width: Int, height: Int, ofType: T.Type)

Initializes a new fast Fourier transform instance for 2D FFT.

### Instance Methods

func transform&lt;T>(input: T, output: inout T, direction: vDSP.FourierTransformDirection)

Computes an out-of-place 2D fast Fourier transform.

## Relationships

### Inherits From

- vDSP.FFT

## See Also

### Objects that Simplify FFTs

class FFT

A 1D single- and double-precision fast Fourier transform.

enum FourierTransformDirection

Fast Fourier transform directions.

enum Radix

Fast Fourier transform radices.

