

- Combine
- Publishers
- Publishers.FlatMap
-  maxPublishers 

Instance Property

# maxPublishers

The maximum number of concurrent publisher subscriptions

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let maxPublishers: Subscribers.Demand
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let transform: (Upstream.Output) -> NewPublisher

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

