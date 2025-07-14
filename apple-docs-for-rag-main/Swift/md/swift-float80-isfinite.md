

- Swift
- Float80
-  isFinite 

Instance Property

# isFinite

A Boolean value indicating whether this instance is finite.

macOS 10.10+

``` source
var isFinite: Bool { get }
```

## Discussion

All values other than NaN and infinity are considered finite, whether normal or subnormal. For NaN, both `isFinite` and `isInfinite` are false.

