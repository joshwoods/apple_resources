

- Combine
- Subscribers
- Subscribers.Demand
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether a demand requests the given number of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Subscribers.Demand, rhs: Int) -> Bool
```

## Discussion

An `.unlimited` demand doesn’t match any integer.

## See Also

### Comparing Demands

static func == (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func == (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether a given number of elements matches the request of a given demand.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func != (Subscribers.Demand, Int) -> Bool

Returns a Boolean value that indicates whether a demand isn’t equal to an integer.

static func != (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether an integer is unequal to a demand.

