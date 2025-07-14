

- Combine
- Publishers
- Publishers.FlatMap
-  init(upstream:maxPublishers:transform:) 

Initializer

# init(upstream:maxPublishers:transform:)

Creates a publisher that transforms elements from an upstream publisher into a new publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    maxPublishers: Subscribers.Demand,
    transform: @escaping (Upstream.Output) -> NewPublisher
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`maxPublishers`  

The maximum number of concurrent publisher subscriptions.

`transform`  

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

