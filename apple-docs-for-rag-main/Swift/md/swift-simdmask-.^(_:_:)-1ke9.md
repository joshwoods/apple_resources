

- Swift
- SIMDMask
-  .^(\_:\_:) 

Operator

# .^(\_:\_:)

A vector mask that is the pointwise exclusive or of the inputs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func .^ (a: Bool, b: SIMDMask) -> SIMDMask
```

Available when `Storage` conforms to `SIMD`, `Storage.Scalar` conforms to `FixedWidthInteger`, and `Storage.Scalar` conforms to `SignedInteger`.

## Discussion

Equivalent to `a ? .!b : b`.

