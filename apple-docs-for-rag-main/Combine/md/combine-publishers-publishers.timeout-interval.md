

- Combine
- Publishers
- Publishers.Timeout
-  interval 

Instance Property

# interval

The maximum time interval the publisher can go without emitting an element, expressed in the time system of the scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let interval: Context.SchedulerTimeType.Stride
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let scheduler: Context

The scheduler on which to deliver events.

let options: Context.SchedulerOptions?

Scheduler options that customize the delivery of elements.

let customError: (() -> Publishers.Timeout&lt;Upstream, Context>.Failure)?

A closure that executes if the publisher times out. The publisher sends the failure returned by this closure to the subscriber as the reason for termination.

