

- Swift
- Dictionary
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: [Key : Value], rhs: [Key : Value]) -> Bool
```

Available when `Key` conforms to `Hashable` and `Value` conforms to `Equatable`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing Dictionaries

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

