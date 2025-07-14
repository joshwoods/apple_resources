

- Swift
- Float
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance from the given value, rounded to the closest possible representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ value: Source) where Source : BinaryFloatingPoint
```

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

## See Also

### Converting Floating-Point Values

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

init(Double)

Creates a new instance that approximates the given value.

init(Float)

Creates a new instance initialized to the given value.

init(Float80)

Creates a new instance that approximates the given value.

init(CGFloat)

init(Float16)

Creates a new instance that approximates the given value.

init(signOf: Float, magnitudeOf: Float)

Creates a new floating-point value using the sign of one value and the magnitude of another.

init(sign: FloatingPointSign, exponent: Int, significand: Float)

Creates a new value from the given sign, exponent, and significand.

init(truncating: NSNumber)

