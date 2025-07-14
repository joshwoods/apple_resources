

- Accelerate
- vDSP
-  phase(\_:result:) 

Type Method

# phase(\_:result:)

Calculates the double-precision element-wise phase values, in radians, of the supplied complex vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func phase(
    _ splitComplex: DSPDoubleSplitComplex,
    result: inout V
) where V : AccelerateMutableBuffer, V.Element == Double
```

## See Also

### Single-Vector Phase Computation

static func phase&lt;V>(DSPSplitComplex, result: inout V)

Calculates the single-precision element-wise phase values, in radians, of the supplied complex vector.

