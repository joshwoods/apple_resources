

- Swift
- Double
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance that approximates the given value.

macOS 10.10+

``` source
init(_ other: Float80)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is rounded to a representable value, if necessary. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Float80 = 21.25
let y = Double(x)
// y == 21.25

let z = Double(Float80.nan)
// z.isNaN == true
```

## See Also

### Converting Floating-Point Values

init&lt;Source>(Source)

Creates a new instance from the given value, rounded to the closest possible representation.

init(Double)

Creates a new instance initialized to the given value.

init(Float)

Creates a new instance that approximates the given value.

init(Float16)

Creates a new instance that approximates the given value.

init(CGFloat)

init(sign: FloatingPointSign, exponent: Int, significand: Double)

Creates a new value from the given sign, exponent, and significand.

init(signOf: Double, magnitudeOf: Double)

Creates a new floating-point value using the sign of one value and the magnitude of another.

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

init(truncating: NSNumber)

