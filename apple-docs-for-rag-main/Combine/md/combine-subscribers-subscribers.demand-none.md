

- Combine
- Subscribers
- Subscribers.Demand
-  none 

Type Property

# none

A request for no elements from the publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let none: Subscribers.Demand
```

## Discussion

This is equivalent to `Demand.max(0)`.

## See Also

### Using Special Demands

static let unlimited: Subscribers.Demand

A request for as many values as the publisher can produce.

