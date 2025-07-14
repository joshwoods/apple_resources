

- Metal
- MTLMathMode
-  MTLMathMode.relaxed 

Case

# MTLMathMode.relaxed

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math, while honoring Inf/NaN.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case relaxed
```

## Discussion

This is the default for Apple silicon devices.

## See Also

### Modes

case fast

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math.

case safe

An indicator of the mode the compiler uses to disable unsafe floating-point optimizations by preventing the compiler from making any transformations that could affect the results.

