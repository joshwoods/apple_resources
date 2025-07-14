

- Metal
- MTLMathMode
-  MTLMathMode.fast 

Case

# MTLMathMode.fast

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case fast
```

## Discussion

This is the default for Intel and AMD devices.

## See Also

### Modes

case relaxed

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math, while honoring Inf/NaN.

case safe

An indicator of the mode the compiler uses to disable unsafe floating-point optimizations by preventing the compiler from making any transformations that could affect the results.

