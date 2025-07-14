

- Combine
- Publishers
-  Publishers.Debounce 

Structure

# Publishers.Debounce

A publisher that publishes elements only after a specified time interval elapses between events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Debounce where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Debounce Publisher

init(upstream: Upstream, dueTime: Context.SchedulerTimeType.Stride, scheduler: Context, options: Context.SchedulerOptions?)

Creates a publisher that publishes elements only after a specified time interval elapses between events.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let dueTime: Context.SchedulerTimeType.Stride

The amount of time the publisher should wait before publishing an element.

let scheduler: Context

The scheduler on which this publisher delivers elements.

let options: Context.SchedulerOptions?

Scheduler options that customize this publisher’s delivery of elements.

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

struct MeasureInterval

A publisher that measures and emits the time interval between events received from an upstream publisher.

struct Delay

A publisher that delays delivery of elements and completion to the downstream receiver.

struct Throttle

A publisher that publishes either the most-recent or first element published by the upstream publisher in a specified time interval.

struct Timeout

A publisher that terminates publishing if the upstream publisher exceeds a specified time interval without producing an element.

