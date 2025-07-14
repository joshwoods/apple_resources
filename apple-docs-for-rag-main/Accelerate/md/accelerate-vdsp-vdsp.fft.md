

- Accelerate
- vDSP
-  vDSP.FFT 

Class

# vDSP.FFT

A 1D single- and double-precision fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
class FFT where T : vDSP_FourierTransformable
```

## Topics

### Initializers

init?(log2n: vDSP_Length, radix: vDSP.Radix, ofType: T.Type)

Initializes a new fast Fourier transform instance.

### Instance Methods

func forward(input: DSPSplitComplex, output: inout DSPSplitComplex)

Computes an out-of-place forward fast Fourier transform.

func inverse(input: DSPSplitComplex, output: inout DSPSplitComplex)

Computes an out-of-place inverse fast Fourier transform.

func transform&lt;T>(input: T, output: inout T, direction: vDSP.FourierTransformDirection)

Computes an out-of-place fast Fourier transform.

### Variables

var FFT_FORWARD: Int

Forward FFT.

var FFT_INVERSE: Int

Inverse FFT.

var FFT_RADIX2: Int

var FFT_RADIX3: Int

var FFT_RADIX5: Int

var kFFTDirection_Forward: Int

var kFFTDirection_Inverse: Int

var kFFTRadix2: Int

var kFFTRadix3: Int

var kFFTRadix5: Int

## Relationships

### Inherited By

- vDSP.FFT2D

## See Also

### Objects that Simplify FFTs

class FFT2D

A 2D single- and double-precision fast Fourier transform.

enum FourierTransformDirection

Fast Fourier transform directions.

enum Radix

Fast Fourier transform radices.

