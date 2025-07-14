

- Combine
- Subscribers
- Subscribers.Demand
-  ...(\_:) 

Operator

# ...(\_:)

Returns a partial range extending upward from a lower bound.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func ... (minimum: Self) -> PartialRangeFrom
```

## Parameters 

`minimum`  

The lower bound for the range.

## Discussion

Use the postfix range operator (postfix `...`) to create a partial range of any type that conforms to the `Comparable` protocol. This example creates a `PartialRangeFrom` instance that includes any value greater than or equal to `5.0`.

```
let atLeastFive = 5.0...

atLeastFive.contains(4.0)     // false
atLeastFive.contains(5.0)     // true
atLeastFive.contains(6.0)     // true
```

You can use this type of partial range of a collection’s indices to represent the range from the partial range’s lower bound up to the end of the collection.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[3...])
// Prints "[40, 50, 60, 70]"
```

Precondition

`minimum` must compare equal to itself (i.e. cannot be NaN).

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

static func -= (inout Subscribers.Demand, Int)

Subtracts an integer from a demand, and assigns the result to the demand.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

