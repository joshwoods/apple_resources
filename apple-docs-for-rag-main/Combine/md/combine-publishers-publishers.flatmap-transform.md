

- Combine
- Publishers
- Publishers.FlatMap
-  transform 

Instance Property

# transform

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let transform: (Upstream.Output) -> NewPublisher
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let maxPublishers: Subscribers.Demand

The maximum number of concurrent publisher subscriptions

