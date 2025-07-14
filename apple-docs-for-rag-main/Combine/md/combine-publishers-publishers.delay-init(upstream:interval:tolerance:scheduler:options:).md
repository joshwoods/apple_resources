

- Combine
- Publishers
- Publishers.Delay
-  init(upstream:interval:tolerance:scheduler:options:) 

Initializer

# init(upstream:interval:tolerance:scheduler:options:)

Creates a publisher that delays delivery of elements and completion to the downstream receiver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    interval: Context.SchedulerTimeType.Stride,
    tolerance: Context.SchedulerTimeType.Stride,
    scheduler: Context,
    options: Context.SchedulerOptions? = nil
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives its elements.

`interval`  

The amount of time to delay.

`tolerance`  

The allowed tolerance in delivering delayed events. The `Delay` publisher may deliver elements this much sooner or later than the interval specifies.

`scheduler`  

The scheduler to deliver the delayed events.

`options`  

Options relevant to the scheduler’s behavior.

