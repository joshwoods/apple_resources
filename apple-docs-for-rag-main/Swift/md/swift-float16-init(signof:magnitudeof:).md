

- Swift
- Float16
-  init(signOf:magnitudeOf:) 

Initializer

# init(signOf:magnitudeOf:)

Creates a new floating-point value using the sign of one value and the magnitude of another.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    signOf sign: Float16,
    magnitudeOf mag: Float16
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

