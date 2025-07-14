

- Swift
- DiscontiguousSlice
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func == (lhs: DiscontiguousSlice, rhs: DiscontiguousSlice) -> Bool
```

Available when `Base` conforms to `Collection` and `Base.Element` conforms to `Equatable`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

