

- Metal Performance Shaders Graph
- MPSGraphFFTDescriptor
-  roundToOddHermitean 

Instance Property

# roundToOddHermitean

A parameter which controls how graph rounds the output tensor size for a Hermitean-to-real Fourier transform.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var roundToOddHermitean: Bool { get set }
```

## Discussion

If set to `YES` then MPSGraph rounds the last output dimension of the result tensor in HermiteanToRealFFT(_:axesTensor:descriptor:name:) to an odd value. Has no effect in the other Fourier transform operations. Default value: `NO`.

