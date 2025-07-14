

- Foundation
- RunLoop
-  RunLoop.SchedulerTimeType 

Structure

# RunLoop.SchedulerTimeType

The scheduler time type that the run loop uses.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SchedulerTimeType
```

## Topics

### Creating Scheduler Times

init(Date)

Initializes a run loop scheduler time with the given date.

### Working with Scheduler Time Intervals

struct Stride

The interval by which run loop times advance.

func advanced(by: RunLoop.SchedulerTimeType.Stride) -> RunLoop.SchedulerTimeType

Returns a run loop scheduler time calculated by advancing this instance’s time by the given interval.

func distance(to: RunLoop.SchedulerTimeType) -> RunLoop.SchedulerTimeType.Stride

Returns the distance to another run loop scheduler time.

### Inspecting Properties

var date: Date

The date this type represents.

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

A set of options that affect the operation of the run loop scheduler.

