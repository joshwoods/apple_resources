

- Combine
- Scheduler
-  SchedulerOptions 

Associated Type

# SchedulerOptions

A type that defines options accepted by the scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype SchedulerOptions
```

**Required**

## Discussion

This type is freely definable by each `Scheduler`. Typically, operations that take a `Scheduler` parameter will also take `SchedulerOptions`.

## See Also

### Declaring Scheduler Timekeeping and Options

associatedtype SchedulerTimeType : Strideable

Describes an instant in time for this scheduler.

**Required**

