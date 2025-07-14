

- Combine
- Subscribers
- Subscribers.Demand
-  \>(\_:\_:) 

Operator

# \>(\_:\_:)

Returns a Boolean that indicates whether the demand requests more than the given number of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func > (lhs: Subscribers.Demand, rhs: Int) -> Bool
```

## Discussion

If `lhs` is `.unlimited`, then the result is always `true`. Otherwise, the operator compares the demand’s `max` value to `rhs`.

