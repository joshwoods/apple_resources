

- Combine
- ImmediateScheduler
-  ImmediateScheduler.SchedulerTimeType 

Structure

# ImmediateScheduler.SchedulerTimeType

The time type used by the immediate scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SchedulerTimeType
```

## Topics

### Declaring a Scheduler Timekeeping System

struct Stride

The increment by which the immediate scheduler counts time.

### Calculating Time Offsets

func advanced(by: ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType

Advances the time by the specified amount; this is meaningless in the context of an immediate scheduler.

func distance(to: ImmediateScheduler.SchedulerTimeType) -> ImmediateScheduler.SchedulerTimeType.Stride

Returns the distance to another immediate scheduler time; this distance is always `0` in the context of an immediate scheduler.

### Comparing Scheduler Times

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable
- Strideable

## See Also

### Declaring Scheduler Timekeeping and Options

typealias SchedulerOptions

A type that defines options accepted by the immediate scheduler.

