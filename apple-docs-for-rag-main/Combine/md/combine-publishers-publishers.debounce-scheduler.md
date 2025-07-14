

- Combine
- Publishers
- Publishers.Debounce
-  scheduler 

Instance Property

# scheduler

The scheduler on which this publisher delivers elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let scheduler: Context
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let dueTime: Context.SchedulerTimeType.Stride

The amount of time the publisher should wait before publishing an element.

let options: Context.SchedulerOptions?

Scheduler options that customize this publisher’s delivery of elements.

