

- Dispatch
- DispatchQueue
-  DispatchQueue.SchedulerOptions 

Structure

# DispatchQueue.SchedulerOptions

A set of options that affect the operation of the dispatch queue scheduler.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct SchedulerOptions
```

## Topics

### Creating Dispatch Queue Scheduler Options

init(qos: DispatchQoS, flags: DispatchWorkItemFlags, group: DispatchGroup?)

Creates a dispatch queue scheduler options instance with the given options.

### Inspecting Scheduler Options

var qos: DispatchQoS

The dispatch queue quality of service.

var flags: DispatchWorkItemFlags

The dispatch queue work item flags.

var group: DispatchGroup?

The dispatch group, if any, to use when performing actions.

## Relationships

### Conforms To

- Sendable

## See Also

### Scheduling Combine Publishers

struct SchedulerTimeType

The scheduler time type used by the dispatch queue.

