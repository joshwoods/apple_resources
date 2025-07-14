

- Accelerate
- vDSP_SplitComplexFloat
-  transform2D(fftSetup:width:height:source:destination:direction:) 

Type Method

# transform2D(fftSetup:width:height:source:destination:direction:)

Performs a 2D fast Fourier transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func transform2D(
    fftSetup: OpaquePointer,
    width: Int,
    height: Int,
    source: UnsafePointer,
    destination: UnsafeMutablePointer,
    direction: vDSP.FourierTransformDirection
)
```

