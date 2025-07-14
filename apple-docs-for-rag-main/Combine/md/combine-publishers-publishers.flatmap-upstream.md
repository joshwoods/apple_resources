

- Combine
- Publishers
- Publishers.FlatMap
-  upstream 

Instance Property

# upstream

The publisher from which this publisher receives elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let maxPublishers: Subscribers.Demand

The maximum number of concurrent publisher subscriptions

let transform: (Upstream.Output) -> NewPublisher

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

