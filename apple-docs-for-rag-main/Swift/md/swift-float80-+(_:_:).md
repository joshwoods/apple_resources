

- Swift
- Float80
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Adds two values and produces their sum, rounded to a representable value.

macOS 10.10+

``` source
static func + (lhs: Float80, rhs: Float80) -> Float80
```

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

## Discussion

The addition operator (`+`) calculates the sum of its two arguments. For example:

```
let x = 1.5
let y = x + 2.25
// y == 3.75
```

The `+` operator implements the addition operation defined by the IEEE 754 specification.

