

- Combine
- Publishers
-  Publishers.MapError 

Structure

# Publishers.MapError

A publisher that converts any failure from the upstream publisher into a new error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MapError where Upstream : Publisher, Failure : Error
```

## Topics

### Creating a Map Error Publisher

init(upstream: Upstream, (Upstream.Failure) -> Failure)

init(upstream: Upstream, transform: (Upstream.Failure) -> Failure)

Creates a publisher that converts any failure from the upstream publisher into a new error.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let transform: (Upstream.Failure) -> Failure

The closure that converts the upstream failure into a new error.

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

struct Scan

A publisher that transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

struct TryScan

A publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

struct SetFailureType

A publisher that appears to send a specified failure type.

