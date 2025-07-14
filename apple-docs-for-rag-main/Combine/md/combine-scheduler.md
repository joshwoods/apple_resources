

- Combine
-  Scheduler 

Protocol

# Scheduler

A protocol that defines when and how to execute a closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Scheduler
```

## Mentioned in 

Receiving and Handling Events with Combine

## Overview

You can use a scheduler to execute code as soon as possible, or after a future date. Individual scheduler implementations use whatever time-keeping system makes sense for them. Schedulers express this as their `SchedulerTimeType`. Since this type conforms to SchedulerTimeIntervalConvertible, you can always express these times with the convenience functions like `.milliseconds(500)`. Schedulers can accept options to control how they execute the actions passed to them. These options may control factors like which threads or dispatch queues execute the actions.

## Topics

### Declaring Scheduler Timekeeping and Options

associatedtype SchedulerTimeType : Strideable

Describes an instant in time for this scheduler.

**Required**

associatedtype SchedulerOptions

A type that defines options accepted by the scheduler.

**Required**

### Accessing Scheduler Time Properties

var minimumTolerance: Self.SchedulerTimeType.Stride

The minimum tolerance allowed by the scheduler.

**Required**

var now: Self.SchedulerTimeType

This scheduler’s definition of the current moment in time.

**Required**

### Scheduling Actions

func schedule(() -> Void)

Performs the action at the next possible opportunity, without options.

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

## Relationships

### Conforming Types

- ImmediateScheduler

## See Also

### Schedulers

struct ImmediateScheduler

A scheduler for performing synchronous actions.

protocol SchedulerTimeIntervalConvertible

A protocol that provides a scheduler with an expression for relative time.

