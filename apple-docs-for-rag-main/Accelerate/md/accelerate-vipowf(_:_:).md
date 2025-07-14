

- Accelerate
-  vipowf(\_:\_:) 

Function

# vipowf(\_:\_:)

For each vector element, calculates `X` to the integer power of `Y`.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vipowf(
    _: vFloat,
    _: vSInt32
) -> vFloat
```

## See Also

### Power Functions (from vfp.h)

func vpowf(vFloat, vFloat) -> vFloat

For each vector element, calculates `X` to the floating-point power of `Y`. The result is more accurate than using exp(log(`X`)\*`Y`).

