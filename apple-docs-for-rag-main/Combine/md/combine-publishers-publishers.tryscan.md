

- Combine
- Publishers
-  Publishers.TryScan 

Structure

# Publishers.TryScan

A publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryScan where Upstream : Publisher
```

## Topics

### Creating a Try Scan Publisher

init(upstream: Upstream, initialResult: Output, nextPartialResult: (Output, Upstream.Output) throws -> Output)

Creates a publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher that this publisher receives elements from.

let initialResult: Output

The previous result returned by the `nextPartialResult` closure.

let nextPartialResult: (Output, Upstream.Output) throws -> Output

An error-throwing closure that takes as its arguments the previous value returned by the closure and the next element emitted from the upstream publisher.

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

struct TryMap

A publisher that transforms all elements from the upstream publisher with a provided error-throwing closure.

struct MapError

A publisher that converts any failure from the upstream publisher into a new error.

struct Scan

A publisher that transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

struct SetFailureType

A publisher that appears to send a specified failure type.

