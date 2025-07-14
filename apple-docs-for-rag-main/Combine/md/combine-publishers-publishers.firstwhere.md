

- Combine
- Publishers
-  Publishers.FirstWhere 

Structure

# Publishers.FirstWhere

A publisher that only publishes the first element of a stream to satisfy a predicate closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct FirstWhere where Upstream : Publisher
```

## Topics

### Creating a First-Where Publisher

init(upstream: Upstream, predicate: (Publishers.FirstWhere&lt;Upstream>.Output) -> Bool)

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Instance Properties

let predicate: (Publishers.FirstWhere&lt;Upstream>.Output) -> Bool

The closure that determines whether to publish an element.

let upstream: Upstream

The publisher from which this publisher receives elements.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Selecting Specific Elements

struct First

A publisher that publishes the first element of a stream, then finishes.

struct TryFirstWhere

A publisher that only publishes the first element of a stream to satisfy a throwing predicate closure.

struct Last

A publisher that waits until after the stream finishes, and then publishes the last element of the stream.

struct LastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies a predicate closure.

struct TryLastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies an error-throwing predicate closure.

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

