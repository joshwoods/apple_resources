

- Combine
- Publishers
-  Publishers.CollectByTime 

Structure

# Publishers.CollectByTime

A publisher that buffers and periodically publishes its items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CollectByTime where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Collect by Time Publisher

init(upstream: Upstream, strategy: Publishers.TimeGroupingStrategy&lt;Context>, options: Context.SchedulerOptions?)

Creates a publisher that buffers and periodically publishes its items.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher that this publisher receives elements from.

let strategy: Publishers.TimeGroupingStrategy&lt;Context>

The strategy with which to collect and publish elements.

let options: Context.SchedulerOptions?

Scheduler options to use for the strategy.

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

enum TimeGroupingStrategy

A strategy for collecting received elements.

struct IgnoreOutput

A publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

struct Reduce

A publisher that applies a closure to all received elements and produces an accumulated value when the upstream publisher finishes.

struct TryReduce

A publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

