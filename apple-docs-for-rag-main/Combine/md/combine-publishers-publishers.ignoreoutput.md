

- Combine
- Publishers
-  Publishers.IgnoreOutput 

Structure

# Publishers.IgnoreOutput

A publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct IgnoreOutput where Upstream : Publisher
```

## Topics

### Creating an Ignore Output Publisher

init(upstream: Upstream)

Creates a publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finish or failed).

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

### Comparing Publishers

static func == (Publishers.IgnoreOutput&lt;Upstream>, Publishers.IgnoreOutput&lt;Upstream>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
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

struct Reduce

A publisher that applies a closure to all received elements and produces an accumulated value when the upstream publisher finishes.

struct TryReduce

A publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

