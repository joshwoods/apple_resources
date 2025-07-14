

- Swift
- Comparable
-  \

Operator

# \

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func  Bool
```

**Required** Default implementations provided.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

This function is the only requirement of the `Comparable` protocol. The remainder of the relational operator functions are implemented by the standard library for any type that conforms to `Comparable`.

## Default Implementations

### Comparable Implementations

static func &lt; &lt;RHS>(Self, RHS) -> Bool

static func &lt; (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func &lt; &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func &lt; (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

