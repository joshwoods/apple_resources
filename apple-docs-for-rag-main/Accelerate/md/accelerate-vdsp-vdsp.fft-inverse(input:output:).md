

- Accelerate
- vDSP
- vDSP.FFT
-  inverse(input:output:) 

Instance Method

# inverse(input:output:)

Computes an out-of-place inverse fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func inverse(
    input: DSPSplitComplex,
    output: inout DSPSplitComplex
)
```

## See Also

### Instance Methods

func forward(input: DSPSplitComplex, output: inout DSPSplitComplex)

Computes an out-of-place forward fast Fourier transform.

func transform&lt;T>(input: T, output: inout T, direction: vDSP.FourierTransformDirection)

Computes an out-of-place fast Fourier transform.

