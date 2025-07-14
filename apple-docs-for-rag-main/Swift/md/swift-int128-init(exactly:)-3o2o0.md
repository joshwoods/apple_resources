

- Swift
- Int128
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance from the given integer, if it can be represented exactly.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(exactly source: T) where T : BinaryInteger
```

## Parameters 

`source`  

A value to convert to this type.

## Discussion

If the value passed as `source` is not representable exactly, the result is `nil`. In the following example, the constant `x` is successfully created from a value of `100`, while the attempt to initialize the constant `y` from `1_000` fails because the `Int8` type can represent `127` at maximum:

```
let x = Int8(exactly: 100)
// x == Optional(100)
let y = Int8(exactly: 1_000)
// y == nil
```

