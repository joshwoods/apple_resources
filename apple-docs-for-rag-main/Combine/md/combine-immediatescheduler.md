

- Combine
-  ImmediateScheduler 

Structure

# ImmediateScheduler

A scheduler for performing synchronous actions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ImmediateScheduler
```

## Overview

You can only use this scheduler for immediate actions. If you attempt to schedule actions after a specific date, this scheduler ignores the date and performs them immediately.

## Topics

### Declaring Scheduler Timekeeping and Options

struct SchedulerTimeType

The time type used by the immediate scheduler.

typealias SchedulerOptions

A type that defines options accepted by the immediate scheduler.

### Accessing Scheduler Time Properties

var minimumTolerance: ImmediateScheduler.SchedulerTimeType.Stride

The minimum tolerance allowed by the immediate scheduler.

var now: ImmediateScheduler.SchedulerTimeType

The immediate scheduler’s definition of the current moment in time.

### Using the Shared Scheduler

static let shared: ImmediateScheduler

The shared instance of the immediate scheduler.

### Scheduling Actions

func schedule(() -> Void)

Performs the action at the next possible opportunity, without options.

func schedule(after: Self.SchedulerTimeType, () -> Void)

Performs the action at some time after the specified date, using the scheduler’s minimum tolerance.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, using minimum tolerance possible for this Scheduler.

func schedule(after: Self.SchedulerTimeType, interval: Self.SchedulerTimeType.Stride, tolerance: Self.SchedulerTimeType.Stride, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, taking into account tolerance if possible.

func schedule(after: ImmediateScheduler.SchedulerTimeType, interval: ImmediateScheduler.SchedulerTimeType.Stride, tolerance: ImmediateScheduler.SchedulerTimeType.Stride, options: ImmediateScheduler.SchedulerOptions?, () -> Void) -> any Cancellable

Performs the action at some time after the specified date, at the specified frequency, optionally taking into account tolerance if possible.

func schedule(after: Self.SchedulerTimeType, tolerance: Self.SchedulerTimeType.Stride, () -> Void)

Performs the action at some time after the specified date.

func schedule(after: ImmediateScheduler.SchedulerTimeType, tolerance: ImmediateScheduler.SchedulerTimeType.Stride, options: ImmediateScheduler.SchedulerOptions?, () -> Void)

Performs the action at some time after the specified date.

func schedule(options: ImmediateScheduler.SchedulerOptions?, () -> Void)

Performs the action at the next possible opportunity.

### Default Implementations

Scheduler Implementations

## Relationships

### Conforms To

- Scheduler

## See Also

### Schedulers

protocol Scheduler

A protocol that defines when and how to execute a closure.

protocol SchedulerTimeIntervalConvertible

A protocol that provides a scheduler with an expression for relative time.

