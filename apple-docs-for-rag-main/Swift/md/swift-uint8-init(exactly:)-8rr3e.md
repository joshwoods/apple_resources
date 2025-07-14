

- Swift
- UInt8
-  init(exactly:) 

Initializer

# init(exactly:)

Creates an integer from the given floating-point value, if it can be represented exactly.

macOS 10.10+

``` source
init?(exactly source: Float80)
```

## Parameters 

`source`  

A floating-point value to convert to an integer.

## Discussion

If the value passed as `source` is not representable exactly, the result is `nil`. In the following example, the constant `x` is successfully created from a value of `21.0`, while the attempt to initialize the constant `y` from `21.5` fails:

```
let x = Int(exactly: 21.0)
// x == Optional(21)
let y = Int(exactly: 21.5)
// y == nil
```

