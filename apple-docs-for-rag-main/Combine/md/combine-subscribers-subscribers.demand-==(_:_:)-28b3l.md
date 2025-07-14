

- Combine
- Subscribers
- Subscribers.Demand
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (a: Subscribers.Demand, b: Subscribers.Demand) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing Demands

static func == (Subscribers.Demand, Int) -> Bool

Returns a Boolean value that indicates whether a demand requests the given number of elements.

static func == (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether a given number of elements matches the request of a given demand.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func != (Subscribers.Demand, Int) -> Bool

Returns a Boolean value that indicates whether a demand isn’t equal to an integer.

static func != (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether an integer is unequal to a demand.

