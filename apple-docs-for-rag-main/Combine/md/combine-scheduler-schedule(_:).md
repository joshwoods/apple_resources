

- Combine
- Scheduler
-  schedule(\_:) 

Instance Method

# schedule(\_:)

Performs the action at the next possible opportunity, without options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func schedule(_ action: @escaping () -> Void)
```

## See Also

### Scheduling Actions

func schedule(after: Self.SchedulerTimeType, () -> Void)

Performs the action at some time after the specified date, using the scheduler’s minimum tolerance.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, using minimum tolerance possible for this Scheduler.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, tolerance: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, taking into account tolerance if possible.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, tolerance: Self.SchedulerTimeType.Stride, options: Self.SchedulerOptions?, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, optionally taking into account tolerance if possible.

**Required**

func schedule(after: Self.SchedulerTimeType, tolerance: Self.SchedulerTimeType.Stride, () -> Void)

Performs the action at some time after the specified date.

func schedule(after: Self.SchedulerTimeType, tolerance: Self.SchedulerTimeType.Stride, options: Self.SchedulerOptions?, () -> Void)

Performs the action at some time after the specified date.

**Required**

func schedule(options: Self.SchedulerOptions?, () -> Void)

Performs the action at the next possible opportunity.

**Required**

