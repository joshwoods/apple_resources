

- Combine
- Publishers
-  Publishers.TryCompactMap 

Structure

# Publishers.TryCompactMap

A publisher that republishes all non-nil results of calling an error-throwing closure with each received element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryCompactMap where Upstream : Publisher
```

## Topics

### Creating a Try Compact Map Publisher

init(upstream: Upstream, transform: (Upstream.Output) throws -> Output?)

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let transform: (Upstream.Output) throws -> Output?

An error-throwing closure that receives values from the upstream publisher and returns optional values.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Filtering Elements

struct Filter

A publisher that republishes all elements that match a provided closure.

struct TryFilter

A publisher that republishes all elements that match a provided error-throwing closure.

struct CompactMap

A publisher that republishes all non-nil results of calling a closure with each received element.

struct RemoveDuplicates

A publisher that publishes only elements that don’t match the previous element.

struct TryRemoveDuplicates

A publisher that publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

struct ReplaceEmpty

A publisher that replaces an empty stream with a provided element.

struct ReplaceError

A publisher that replaces any errors in the stream with a provided element.

