

- Swift
- Float80
-  init(nan:signaling:) 

Initializer

# init(nan:signaling:)

Creates a NaN (“not a number”) value with the specified payload.

macOS 10.10+

``` source
init(
    nan payload: Float80.RawSignificand,
    signaling: Bool
)
```

## Parameters 

`payload`  

The payload to use for the new NaN value.

`signaling`  

Pass `true` to create a signaling NaN or `false` to create a quiet NaN.

## Discussion

NaN values compare not equal to every value, including themselves. Most operations with a NaN operand produce a NaN result. Don’t use the equal-to operator (`==`) to test whether a value is NaN. Instead, use the value’s `isNaN` property.

```
let x = Float80(nan: 0, signaling: false)
print(x == .nan)
// Prints "false"
print(x.isNaN)
// Prints "true"
```

