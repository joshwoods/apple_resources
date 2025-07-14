

- Combine
- Publishers
-  Publishers.FlatMap 

Structure

# Publishers.FlatMap

A publisher that transforms elements from an upstream publisher into a new publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct FlatMap where NewPublisher : Publisher, Upstream : Publisher, NewPublisher.Failure == Upstream.Failure
```

## Topics

### Creating a Flat Map Publisher

init(upstream: Upstream, maxPublishers: Subscribers.Demand, transform: (Upstream.Output) -> NewPublisher)

Creates a publisher that transforms elements from an upstream publisher into a new publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let maxPublishers: Subscribers.Demand

The maximum number of concurrent publisher subscriptions

let transform: (Upstream.Output) -> NewPublisher

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Republishing Elements by Subscribing to New Publishers

struct SwitchToLatest

A publisher that flattens nested publishers.

