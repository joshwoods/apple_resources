

- Accelerate
- vDSP
- vDSP.FFT2D
-  transform(input:output:direction:) 

Instance Method

# transform(input:output:direction:)

Computes an out-of-place 2D fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
override func transform(
    input: T,
    output: inout T,
    direction: vDSP.FourierTransformDirection
) where T : vDSP_FourierTransformable
```

