

- Accelerate
- vDSP_DFTFunctions
-  transform(dftSetup:inputReal:inputImaginary:outputReal:outputImaginary:) Deprecated

Type Method

# transform(dftSetup:inputReal:inputImaginary:outputReal:outputImaginary:)

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+Mac Catalyst

``` source
static func transform(
    dftSetup: OpaquePointer,
    inputReal: U,
    inputImaginary: U,
    outputReal: inout V,
    outputImaginary: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, Self.Scalar == U.Element, U.Element == V.Element
```

**Required**

Deprecated

Use `vDSP.DiscreteFourierTransform`.

