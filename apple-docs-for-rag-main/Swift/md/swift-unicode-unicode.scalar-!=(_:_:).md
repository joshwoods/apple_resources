

- Swift
- Unicode
- Unicode.Scalar
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

## See Also

### Comparing Scalars

static func == (Unicode.Scalar, Unicode.Scalar) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Unicode.Scalar, Unicode.Scalar) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

