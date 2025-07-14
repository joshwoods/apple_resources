

- Combine
- Publishers
-  Publishers.MeasureInterval 

Structure

# Publishers.MeasureInterval

A publisher that measures and emits the time interval between events received from an upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MeasureInterval where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Measure Interval Publisher

init(upstream: Upstream, scheduler: Context)

Creates a publisher that measures and emits the time interval between events received from an upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let scheduler: Context

The scheduler used for tracking the timing of events.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Controlling Timing

struct Debounce

A publisher that publishes elements only after a specified time interval elapses between events.

struct Delay

A publisher that delays delivery of elements and completion to the downstream receiver.

struct Throttle

A publisher that publishes either the most-recent or first element published by the upstream publisher in a specified time interval.

struct Timeout

A publisher that terminates publishing if the upstream publisher exceeds a specified time interval without producing an element.

