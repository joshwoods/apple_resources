

- Metal
- MTLMathMode
-  MTLMathMode.safe 

Case

# MTLMathMode.safe

An indicator of the mode the compiler uses to disable unsafe floating-point optimizations by preventing the compiler from making any transformations that could affect the results.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case safe
```

## See Also

### Modes

case fast

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math.

case relaxed

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math, while honoring Inf/NaN.

