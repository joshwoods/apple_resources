

- Combine
- Subscribers
- Subscribers.Demand
-  \>(\_:\_:) 

Operator

# \>(\_:\_:)

Returns a Boolean that indicates whether the first demand requests more elements than the second.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func > (lhs: Subscribers.Demand, rhs: Subscribers.Demand) -> Bool
```

## Discussion

If both sides are `.unlimited`, the result is always `false`. If `lhs` is `.unlimited`, then the result is always `true`. If `rhs` is `.unlimited` then the result is always `false`. Otherwise, this operator compares the demands’ `max` values.

