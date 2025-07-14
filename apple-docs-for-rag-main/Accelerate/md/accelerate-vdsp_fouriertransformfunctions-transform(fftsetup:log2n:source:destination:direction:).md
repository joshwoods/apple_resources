

- Accelerate
- vDSP_FourierTransformFunctions
-  transform(fftSetup:log2n:source:destination:direction:) 

Type Method

# transform(fftSetup:log2n:source:destination:direction:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func transform(
    fftSetup: OpaquePointer,
    log2n: vDSP_Length,
    source: UnsafePointer,
    destination: UnsafeMutablePointer,
    direction: vDSP.FourierTransformDirection
)
```

**Required**

