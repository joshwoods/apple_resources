

- Combine
- Publishers
-  Publishers.ContainsWhere 

Structure

# Publishers.ContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the predicate closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ContainsWhere where Upstream : Publisher
```

## Topics

### Creating a Contains Where Publisher

init(upstream: Upstream, predicate: (Upstream.Output) -> Bool)

Creates a publisher that emits a Boolean value upon receiving an element that satisfies the predicate closure.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let predicate: (Upstream.Output) -> Bool

The closure that determines whether the publisher should consider an element as a match.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Applying Matching Criteria to Elements

struct Contains

A publisher that emits a Boolean value when it receives a specific element from its upstream publisher.

struct TryContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the throwing predicate closure.

struct AllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given predicate.

struct TryAllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

