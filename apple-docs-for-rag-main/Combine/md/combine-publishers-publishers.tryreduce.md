

- Combine
- Publishers
-  Publishers.TryReduce 

Structure

# Publishers.TryReduce

A publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryReduce where Upstream : Publisher
```

## Topics

### Creating a Try Reduce Publisher

init(upstream: Upstream, initial: Output, nextPartialResult: (Output, Upstream.Output) throws -> Output)

Creates a publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let initial: Output

The initial value provided on the first-use of the closure.

let nextPartialResult: (Output, Upstream.Output) throws -> Output

An error-throwing closure that takes the previously-accumulated value and the next element from the upstream to produce a new value.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Reducing Elements

struct Collect

A publisher that buffers items.

struct CollectByCount

A publisher that buffers a maximum number of items.

struct CollectByTime

A publisher that buffers and periodically publishes its items.

enum TimeGroupingStrategy

A strategy for collecting received elements.

struct IgnoreOutput

A publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

struct Reduce

A publisher that applies a closure to all received elements and produces an accumulated value when the upstream publisher finishes.

