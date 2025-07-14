

- Swift
- FloatingPoint
-  isFinite 

Instance Property

# isFinite

A Boolean value indicating whether this instance is finite.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFinite: Bool { get }
```

**Required**

## Discussion

All values other than NaN and infinity are considered finite, whether normal or subnormal. For NaN, both `isFinite` and `isInfinite` are false.

