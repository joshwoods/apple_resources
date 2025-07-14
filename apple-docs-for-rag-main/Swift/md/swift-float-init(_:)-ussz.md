

- Swift
- Float
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance that approximates the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(_ other: Float16)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is rounded to a representable value, if necessary. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Float16 = 21.25
let y = Float(x)
// y == 21.25

let z = Float(Float16.nan)
// z.isNaN == true
```

## See Also

### Converting Floating-Point Values

init&lt;Source>(Source)

Creates a new instance from the given value, rounded to the closest possible representation.

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

init(Double)

Creates a new instance that approximates the given value.

init(Float)

Creates a new instance initialized to the given value.

init(Float80)

Creates a new instance that approximates the given value.

init(CGFloat)

init(signOf: Float, magnitudeOf: Float)

Creates a new floating-point value using the sign of one value and the magnitude of another.

init(sign: FloatingPointSign, exponent: Int, significand: Float)

Creates a new value from the given sign, exponent, and significand.

init(truncating: NSNumber)

