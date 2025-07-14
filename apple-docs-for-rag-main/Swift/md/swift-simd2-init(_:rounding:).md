

- Swift
- SIMD2
-  init(\_:rounding:) 

Initializer

# init(\_:rounding:)

Creates a new vector from the given vector, rounding the given vector’s of elements using the specified rounding rule.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    _ other: SIMD2,
    rounding rule: FloatingPointRoundingRule = .towardZero
) where Other : BinaryFloatingPoint, Other : SIMDScalar
```

Available when `Scalar` conforms to `FixedWidthInteger` and `SIMDScalar`.

## Parameters 

`other`  

The vector to convert.

`rule`  

The round rule to use when converting elements of `other.` The default is `.towardZero`.

