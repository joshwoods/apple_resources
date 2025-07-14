

- Swift
- Float80
-  init(signOf:magnitudeOf:) 

Initializer

# init(signOf:magnitudeOf:)

Creates a new floating-point value using the sign of one value and the magnitude of another.

macOS 10.10+

``` source
init(
    signOf sign: Float80,
    magnitudeOf mag: Float80
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

