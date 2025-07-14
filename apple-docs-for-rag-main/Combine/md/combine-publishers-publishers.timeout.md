

- Combine
- Publishers
-  Publishers.Timeout 

Structure

# Publishers.Timeout

A publisher that terminates publishing if the upstream publisher exceeds a specified time interval without producing an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Timeout where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Timeout Publisher

init(upstream: Upstream, interval: Context.SchedulerTimeType.Stride, scheduler: Context, options: Context.SchedulerOptions?, customError: (() -> Publishers.Timeout&lt;Upstream, Context>.Failure)?)

Creates a publisher that terminates publishing if the upstream publisher exceeds the specified time interval without producing an element.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let interval: Context.SchedulerTimeType.Stride

The maximum time interval the publisher can go without emitting an element, expressed in the time system of the scheduler.

let scheduler: Context

The scheduler on which to deliver events.

let options: Context.SchedulerOptions?

Scheduler options that customize the delivery of elements.

let customError: (() -> Publishers.Timeout&lt;Upstream, Context>.Failure)?

A closure that executes if the publisher times out. The publisher sends the failure returned by this closure to the subscriber as the reason for termination.

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

struct Debounce

A publisher that publishes elements only after a specified time interval elapses between events.

struct Delay

A publisher that delays delivery of elements and completion to the downstream receiver.

struct Throttle

A publisher that publishes either the most-recent or first element published by the upstream publisher in a specified time interval.

