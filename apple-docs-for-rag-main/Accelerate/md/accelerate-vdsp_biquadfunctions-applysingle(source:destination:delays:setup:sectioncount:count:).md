

- Accelerate
- vDSP_BiquadFunctions
-  applySingle(source:destination:delays:setup:sectionCount:count:) 

Type Method

# applySingle(source:destination:delays:setup:sectionCount:count:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func applySingle(
    source: U,
    destination: inout V,
    delays: UnsafeMutablePointer,
    setup: vDSP_biquad_Setup,
    sectionCount: vDSP_Length,
    count: vDSP_Length
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, Self.Scalar == U.Element, U.Element == V.Element
```

**Required**

