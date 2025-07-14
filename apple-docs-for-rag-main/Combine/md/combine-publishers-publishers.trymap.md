

- Combine
- Publishers
-  Publishers.TryMap 

Structure

# Publishers.TryMap

A publisher that transforms all elements from the upstream publisher with a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryMap where Upstream : Publisher
```

## Topics

### Creating a Try Map Publisher

init(upstream: Upstream, transform: (Upstream.Output) throws -> Output)

Creates a publisher that transforms all elements from the upstream publisher with a provided error-throwing closure.

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let transform: (Upstream.Output) throws -> Output

The error-throwing closure that transforms elements from the upstream publisher.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Mapping Elements

struct Map

A publisher that transforms all elements from the upstream publisher with a provided closure.

struct MapError

A publisher that converts any failure from the upstream publisher into a new error.

struct Scan

A publisher that transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

struct TryScan

A publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

struct SetFailureType

A publisher that appears to send a specified failure type.

