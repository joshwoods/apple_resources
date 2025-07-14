

- Swift
- SIMDMask
-  random(using:) 

Type Method

# random(using:)

Returns a vector mask with `true` or `false` randomly assigned in each lane, using the given generator as a source for randomness.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random(using generator: inout T) -> SIMDMask where T : RandomNumberGenerator
```

Available when `Storage` conforms to `SIMD`, `Storage.Scalar` conforms to `FixedWidthInteger`, and `Storage.Scalar` conforms to `SignedInteger`.

