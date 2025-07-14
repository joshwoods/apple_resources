

- Accelerate
- vDSP
- vDSP.FFT
-  transform(input:output:direction:) 

Instance Method

# transform(input:output:direction:)

Computes an out-of-place fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func transform(
    input: T,
    output: inout T,
    direction: vDSP.FourierTransformDirection
) where T : vDSP_FourierTransformable
```

## See Also

### Instance Methods

func forward(input: DSPSplitComplex, output: inout DSPSplitComplex)

Computes an out-of-place forward fast Fourier transform.

func inverse(input: DSPSplitComplex, output: inout DSPSplitComplex)

Computes an out-of-place inverse fast Fourier transform.

