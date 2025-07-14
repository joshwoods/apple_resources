

- Swift
- Float
-  init(signOf:magnitudeOf:) 

Initializer

# init(signOf:magnitudeOf:)

Creates a new floating-point value using the sign of one value and the magnitude of another.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    signOf sign: Float,
    magnitudeOf mag: Float
)
```

## Discussion

The following example uses this initializer to create a new `Double` instance with the sign of `a` and the magnitude of `b`:

```
let a = -21.5
let b = 305.15
let c = Double(signOf: a, magnitudeOf: b)
print(c)
// Prints "-305.15"
```

This initializer implements the IEEE 754 `copysign` operation.

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

init(Float16)

Creates a new instance that approximates the given value.

init(sign: FloatingPointSign, exponent: Int, significand: Float)

Creates a new value from the given sign, exponent, and significand.

init(truncating: NSNumber)

