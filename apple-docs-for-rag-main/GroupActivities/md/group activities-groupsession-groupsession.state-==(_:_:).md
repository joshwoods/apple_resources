

- Group Activities
- GroupSession
- GroupSession.State
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func == (lhs: GroupSession.State, rhs: GroupSession.State) -> Bool
```

Available when `ActivityType` conforms to `GroupActivity`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing states

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

