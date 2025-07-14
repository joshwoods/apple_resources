

- Combine
- Subscribers
- Subscribers.Demand
-  -=(\_:\_:) 

Operator

# -=(\_:\_:)

Subtracts an integer from a demand, and assigns the result to the demand.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func -= (lhs: inout Subscribers.Demand, rhs: Int)
```

## Discussion

When subtracting any value from `.unlimited`, the result is still `.unlimited`. A negative demand is impossible; when an operation would result in a negative value, Combine adjusts the value to `.max(0)`.

## See Also

### Performing Mathematical Operations

static func * (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of multiplying a demand by an integer.

static func *= (inout Subscribers.Demand, Int)

Multiplies a demand by an integer, and assigns the result to the demand.

static func + (Subscribers.Demand, Subscribers.Demand) -> Subscribers.Demand

Returns the result of adding two demands. When adding any value to `.unlimited`, the result is `.unlimited`.

static func + (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of adding an integer to a demand.

static func += (inout Subscribers.Demand, Subscribers.Demand)

Adds two demands, and assigns the result to the first demand.

static func += (inout Subscribers.Demand, Int)

Adds an integer to a demand, and assigns the result to the demand.

static func - (Subscribers.Demand, Subscribers.Demand) -> Subscribers.Demand

Returns the result of subtracting one demand from another.

static func - (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of subtracting an integer from a demand.

static func -= (inout Subscribers.Demand, Subscribers.Demand)

Subtracts one demand from another, and assigns the result to the first demand.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

