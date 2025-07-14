

- Foundation
- Measurement
-  \>(\_:\_:) 

Operator

# \>(\_:\_:)

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func > (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

This is the default implementation of the greater-than operator (`>`) for any type that conforms to `Comparable`.

## See Also

### Comparing Measurements

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

static func &lt; &lt;LeftHandSideType, RightHandSideType>(Measurement&lt;LeftHandSideType>, Measurement&lt;RightHandSideType>) -> Bool

Compare two measurements of the same `Unit`.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

