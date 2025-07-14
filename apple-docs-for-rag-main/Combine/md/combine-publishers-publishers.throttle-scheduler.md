

- Combine
- Publishers
- Publishers.Throttle
-  scheduler 

Instance Property

# scheduler

The scheduler on which to publish elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let scheduler: Context
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let interval: Context.SchedulerTimeType.Stride

The interval in which to find and emit the most recent element.

let latest: Bool

A Boolean value indicating whether to publish the most recent element.

