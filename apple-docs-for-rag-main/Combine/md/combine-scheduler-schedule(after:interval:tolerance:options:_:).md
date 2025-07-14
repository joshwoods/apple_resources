

- Combine
- Scheduler
-  schedule(after:interval:tolerance:options:\_:) 

Instance Method

# schedule(after:interval:tolerance:options:\_:)

Performs the action at some time after the specified date, at the specified frequency, optionally taking into account tolerance if possible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func schedule(
    after date: Self.SchedulerTimeType,
    interval: Self.SchedulerTimeType.Stride,
    tolerance: Self.SchedulerTimeType.Stride,
    options: Self.SchedulerOptions?,
    _ action: @escaping () -> Void
) -> any Cancellable
```

**Required**

## See Also

### Scheduling Actions

func schedule(() -> Void)

Performs the action at the next possible opportunity, without options.

func schedule(after: Self.SchedulerTimeType, () -> Void)

Performs the action at some time after the specified date, using the scheduler’s minimum tolerance.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, using minimum tolerance possible for this Scheduler.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, tolerance: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, taking into account tolerance if possible.

func schedule(after: Self.SchedulerTimeType, tolerance: Self.SchedulerTimeType.Stride, () -> Void)

Performs the action at some time after the specified date.

func schedule(after: Self.SchedulerTimeType, tolerance: Self.SchedulerTimeType.Stride, options: Self.SchedulerOptions?, () -> Void)

Performs the action at some time after the specified date.

**Required**

func schedule(options: Self.SchedulerOptions?, () -> Void)

Performs the action at the next possible opportunity.

**Required**

