

- Combine
- Publishers
-  Publishers.AllSatisfy 

Structure

# Publishers.AllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given predicate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AllSatisfy where Upstream : Publisher
```

## Topics

### Creating an All Satisfy Publisher

init(upstream: Upstream, predicate: (Upstream.Output) -> Bool)

Creates a publisher that publishes a single Boolean value that indicates whether all received elements pass a given predicate.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let predicate: (Upstream.Output) -> Bool

A closure that evaluates each received element.

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

struct ContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the predicate closure.

struct TryContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the throwing predicate closure.

struct TryAllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

