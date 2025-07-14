

- Combine
- Subscribers
- Subscribers.Demand
-  ...(\_:\_:) 

Operator

# ...(\_:\_:)

Returns a closed range that contains both of its bounds.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func ... (minimum: Self, maximum: Self) -> ClosedRange
```

## Parameters 

`minimum`  

The lower bound for the range.

`maximum`  

The upper bound for the range.

## Discussion

Use the closed range operator (`...`) to create a closed range of any type that conforms to the `Comparable` protocol. This example creates a `ClosedRange` from “a” up to, and including, “z”.

```
let lowercase = "a"..."z"
print(lowercase.contains("z"))
// Prints "true"
```

Precondition

`minimum 

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

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

