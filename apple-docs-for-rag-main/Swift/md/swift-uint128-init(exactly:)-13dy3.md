

- Swift
- UInt128
-  init(exactly:) 

Initializer

# init(exactly:)

Creates an integer from the given floating-point value, if it can be represented exactly.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(exactly source: T) where T : BinaryFloatingPoint
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

