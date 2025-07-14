

- Accelerate
- vDSP_SplitComplexFloat
-  makeFFTSetup(log2n:radix:) 

Type Method

# makeFFTSetup(log2n:radix:)

Returns a setup structure to perform a fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func makeFFTSetup(
    log2n: vDSP_Length,
    radix: vDSP.Radix
) -> OpaquePointer?
```

