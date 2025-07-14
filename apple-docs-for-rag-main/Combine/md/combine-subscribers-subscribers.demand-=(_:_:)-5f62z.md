

- Combine
- Subscribers
- Subscribers.Demand
-  \

Operator

# \

Returns a Boolean value that indicates a given number of elements is less than or equal the maximum specified by the demand.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func  Bool
```

## Discussion

If `rhs` is `.unlimited`, then the result is always `true`. Otherwise, the operator compares the demand’s `max` value to `lhs`.

