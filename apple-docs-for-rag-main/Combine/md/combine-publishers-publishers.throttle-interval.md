

- Combine
- Publishers
- Publishers.Throttle
-  interval 

Instance Property

# interval

The interval in which to find and emit the most recent element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let interval: Context.SchedulerTimeType.Stride
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let scheduler: Context

The scheduler on which to publish elements.

let latest: Bool

A Boolean value indicating whether to publish the most recent element.

