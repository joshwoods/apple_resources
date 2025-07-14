

- Swift
- Int
-  /=(\_:\_:) 

Operator

# /=(\_:\_:)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func /= (lhs: inout Int, rhs: Int)
```

## Parameters 

`lhs`  

The value to divide.

`rhs`  

The value to divide `lhs` by. `rhs` must not be zero.

## Discussion

For integer types, any remainder of the division is discarded.

```
var x = 21
x /= 5
// x == 4
```

## See Also

### Arithmetic with Assignment

static func += (inout Int, Int)

Adds two values and stores the result in the left-hand-side variable.

static func *= (inout Int, Int)

Multiplies two values and stores the result in the left-hand-side variable.

