

- Swift
- BinaryInteger
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Adds two values and stores the result in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
override static func += (lhs: inout Self, rhs: Self)
```

**Required**

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

## Discussion

The sum of the two arguments must be representable in the arguments’ type. In the following example, the result of `21 + 120` is greater than the maximum representable `Int8` value:

```
var x: Int8 = 21
x += 120
// Overflow error
```

Note

Overflow checking is not performed in `-Ounchecked` builds.

## See Also

### Arithmetic with Assignment

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

**Required**

static func *= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable.

**Required**

static func /= (inout Self, Self)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

**Required**

