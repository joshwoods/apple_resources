

- Combine
- Publishers
- Publishers.Delay
-  upstream 

Instance Property

# upstream

The publisher from which this publisher receives its elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let interval: Context.SchedulerTimeType.Stride

The amount of time to delay.

let tolerance: Context.SchedulerTimeType.Stride

The allowed tolerance in firing delayed events.

let scheduler: Context

The scheduler to deliver the delayed events.

let options: Context.SchedulerOptions?

Options relevant to the scheduler’s behavior.

