

- GLKit
- GLKFogMode
-  GLKFogMode.exp2 

Case

# GLKFogMode.exp2

The fog component is calculated as `exp(-(density * distance)^2)` and clamped to the range `[0.0, 1.0]`.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
case exp2
```

## See Also

### Constants

case exp

The fog component is calculated as `exp(-density * distance)` and clamped to the range `[0.0, 1.0]`.

case linear

The fog component is calculated as `(end - distance) / (end - start)` and clamped to the range `[0.0, 1.0]`.

