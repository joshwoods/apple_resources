

- Combine
- Publishers
-  Publishers.Catch 

Structure

# Publishers.Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Catch where Upstream : Publisher, NewPublisher : Publisher, Upstream.Output == NewPublisher.Output
```

## Topics

### Creating a Catch Publisher

init(upstream: Upstream, handler: (Upstream.Failure) -> NewPublisher)

Creates a publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

let handler: (Upstream.Failure) -> NewPublisher

A closure that accepts the upstream failure as input and returns a publisher to replace the upstream publisher.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Convenience Publishers

struct Sequence

A publisher that publishes a given sequence of elements.

