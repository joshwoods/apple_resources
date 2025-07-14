

- Accelerate
-  vremquof(\_:\_:\_:) 

Function

# vremquof(\_:\_:\_:)

For each vector element, calculates the remainder of `X`/`Y`, according to the SANE standard. It stores into `QUO` the 7 low-order bits of the integer quotient, such that -127 \

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vremquof(
    _: vFloat,
    _: vFloat,
    _: UnsafeMutablePointer
) -> vFloat
```

## See Also

### Remainder Functions (from vfp.h)

func vfmodf(vFloat, vFloat) -> vFloat

For each vector element, calculates `X` modulo `Y`.

func vremainderf(vFloat, vFloat) -> vFloat

For each vector element, calculates the remainder of `X`/`Y`, according to the IEEE 754 floating-point standard.

