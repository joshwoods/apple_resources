

- Accelerate
-  vfmodf(\_:\_:) 

Function

# vfmodf(\_:\_:)

For each vector element, calculates `X` modulo `Y`.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vfmodf(
    _: vFloat,
    _: vFloat
) -> vFloat
```

## See Also

### Remainder Functions (from vfp.h)

func vremainderf(vFloat, vFloat) -> vFloat

For each vector element, calculates the remainder of `X`/`Y`, according to the IEEE 754 floating-point standard.

func vremquof(vFloat, vFloat, UnsafeMutablePointer&lt;vUInt32>) -> vFloat

For each vector element, calculates the remainder of `X`/`Y`, according to the SANE standard. It stores into `QUO` the 7 low-order bits of the integer quotient, such that -127 \

