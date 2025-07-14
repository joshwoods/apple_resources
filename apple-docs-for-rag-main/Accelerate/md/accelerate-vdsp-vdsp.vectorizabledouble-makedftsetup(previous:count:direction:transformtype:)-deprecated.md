

- Accelerate
- vDSP
- vDSP.VectorizableDouble
-  makeDFTSetup(previous:count:direction:transformType:) Deprecated

Type Method

# makeDFTSetup(previous:count:direction:transformType:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func makeDFTSetup(
    previous: vDSP.DFT? = nil,
    count: Int,
    direction: vDSP.FourierTransformDirection,
    transformType: vDSP.DFTTransformType
) -> OpaquePointer? where T : vDSP_FloatingPointDiscreteFourierTransformable
```

Deprecated

Use `vDSP.DiscreteFourierTransform`.

