

- Combine
- ImmediateScheduler
-  Scheduler Implementations 

API Collection

# Scheduler Implementations

## Topics

### Instance Methods

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

