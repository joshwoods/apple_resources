

- Swift
- SIMD2
-  init(\_:) 

Initializer

# init(\_:)

Creates a new vector from the given vector of integers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ other: SIMD2) where Other : FixedWidthInteger, Other : SIMDScalar
```

Available when `Scalar` conforms to `BinaryFloatingPoint` and `SIMDScalar`.

## Parameters 

`other`  

The vector to convert.

