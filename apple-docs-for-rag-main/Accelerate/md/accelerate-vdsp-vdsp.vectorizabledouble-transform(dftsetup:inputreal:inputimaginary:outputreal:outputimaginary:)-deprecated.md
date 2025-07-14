

- Accelerate
- vDSP
- vDSP.VectorizableDouble
-  transform(dftSetup:inputReal:inputImaginary:outputReal:outputImaginary:) Deprecated

Type Method

# transform(dftSetup:inputReal:inputImaginary:outputReal:outputImaginary:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func transform(
    dftSetup: OpaquePointer,
    inputReal: U,
    inputImaginary: U,
    outputReal: inout V,
    outputImaginary: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

Deprecated

Use `vDSP.DiscreteFourierTransform`.

