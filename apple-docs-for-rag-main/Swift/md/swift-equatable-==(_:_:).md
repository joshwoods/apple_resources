

- Swift
- Equatable
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: Self, rhs: Self) -> Bool
```

**Required** Default implementations provided.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## Default Implementations

### DistributedActor Implementations

static func == (Self, Self) -> Bool

A distributed actor’s hash and equality is implemented by directly delegating to its id.

### Equatable Implementations

static func == &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are equal.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two vectors are equal.

static func == &lt;RHS>(Self, RHS) -> Bool

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

## See Also

### Equatable Requirements

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

