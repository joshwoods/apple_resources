

- Swift
- SIMD3
-  init(clamping:) 

Initializer

# init(clamping:)

Creates a new vector from the given vector, clamping the values of the given vector’s elements if necessary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(clamping other: SIMD3) where Other : FixedWidthInteger, Other : SIMDScalar
```

Available when `Scalar` conforms to `FixedWidthInteger` and `SIMDScalar`.

## Parameters 

`other`  

The vector to convert.

