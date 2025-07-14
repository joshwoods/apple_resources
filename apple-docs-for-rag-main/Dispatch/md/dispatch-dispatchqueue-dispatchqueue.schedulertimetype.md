

- Dispatch
- DispatchQueue
-  DispatchQueue.SchedulerTimeType 

Structure

# DispatchQueue.SchedulerTimeType

The scheduler time type used by the dispatch queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct SchedulerTimeType
```

## Topics

### Creating Scheduler Times

init(DispatchTime)

Creates a dispatch queue time type instance.

### Working with Scheduler Time Intervals

func advanced(by: DispatchQueue.SchedulerTimeType.Stride) -> DispatchQueue.SchedulerTimeType

func distance(to: DispatchQueue.SchedulerTimeType) -> DispatchQueue.SchedulerTimeType.Stride

### Inspecting Scheduler Time Properties

var dispatchTime: DispatchTime

The dispatch time represented by this type.

## Relationships

### Conforms To

- Comparable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- Strideable

## See Also

### Scheduling Combine Publishers

struct SchedulerOptions

A set of options that affect the operation of the dispatch queue scheduler.

