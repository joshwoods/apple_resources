

- Combine
- Publishers
-  Publishers.SwitchToLatest 

Structure

# Publishers.SwitchToLatest

A publisher that flattens nested publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SwitchToLatest where P : Publisher, P == Upstream.Output, Upstream : Publisher, P.Failure == Upstream.Failure
```

## Overview

Given a publisher that publishes Publisher instances, the Publishers.SwitchToLatest publisher produces a sequence of events from only the most recent one. For example, given the type `AnyPublisher`, calling `Publisher/switchToLatest()` results in the type `SwitchToLatest`. The downstream subscriber sees a continuous stream of `(Data, URLResponse)` elements from what looks like a single URLSession.DataTaskPublisher even though the elements are coming from different upstream publishers.

When Publishers.SwitchToLatest receives a new publisher from the upstream publisher, it cancels its previous subscription. Use this feature to prevent earlier publishers from performing unnecessary work, such as creating network request publishers from frequently-updating user interface publishers.

## Topics

### Creating a Switch to Latest Publisher

init(upstream: Upstream)

Creates a publisher that “flattens” nested publishers.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

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

struct FlatMap

A publisher that transforms elements from an upstream publisher into a new publisher.

