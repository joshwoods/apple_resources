

- Swift
- Float80
-  /(\_:\_:) 

Operator

# /(\_:\_:)

Returns the quotient of dividing the first value by the second, rounded to a representable value.

macOS 10.10+

``` source
static func / (lhs: Float80, rhs: Float80) -> Float80
```

## Parameters 

`lhs`  

The value to divide.

`rhs`  

The value to divide `lhs` by.

## Discussion

The division operator (`/`) calculates the quotient of the division if `rhs` is nonzero. If `rhs` is zero, the result of the division is infinity, with the sign of the result matching the sign of `lhs`.

```
let x = 16.875
let y = x / 2.25
// y == 7.5

let z = x / 0
// z.isInfinite == true
```

The `/` operator implements the division operation defined by the IEEE 754 specification.

