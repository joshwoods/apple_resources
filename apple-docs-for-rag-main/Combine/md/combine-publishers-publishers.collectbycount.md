

- Combine
- Publishers
-  Publishers.CollectByCount 

Structure

# Publishers.CollectByCount

A publisher that buffers a maximum number of items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CollectByCount where Upstream : Publisher
```

## Topics

### Creating a Collect by Count Publisher

init(upstream: Upstream, count: Int)

Creates a publisher that buffers a maximum number of items.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher that this publisher receives elements from.

let count: Int

The maximum number of received elements to buffer before publishing.

### Comparing Publishers

static func == (Publishers.CollectByCount&lt;Upstream>, Publishers.CollectByCount&lt;Upstream>) -> Bool

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

struct CollectByTime

A publisher that buffers and periodically publishes its items.

enum TimeGroupingStrategy

A strategy for collecting received elements.

struct IgnoreOutput

A publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

struct Reduce

A publisher that applies a closure to all received elements and produces an accumulated value when the upstream publisher finishes.

struct TryReduce

A publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

