

- Swift
- Float16
-  isFinite 

Instance Property

# isFinite

A Boolean value indicating whether this instance is finite.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isFinite: Bool { get }
```

## Discussion

All values other than NaN and infinity are considered finite, whether normal or subnormal. For NaN, both `isFinite` and `isInfinite` are false.

