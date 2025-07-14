

- Swift
- SIMD32
-  wrappedSum() 

Instance Method

# wrappedSum()

Returns the sum of the scalars in the vector, computed with wrapping addition.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func wrappedSum() -> Self.Scalar
```

Available when `Scalar` conforms to `FixedWidthInteger`.

## Discussion

Equivalent to `indices.reduce(into: 0) { $0 &+= self[$1] }`.

