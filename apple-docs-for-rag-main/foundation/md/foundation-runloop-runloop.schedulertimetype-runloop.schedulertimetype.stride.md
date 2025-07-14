

- Foundation
- RunLoop
- RunLoop.SchedulerTimeType
-  RunLoop.SchedulerTimeType.Stride 

Structure

# RunLoop.SchedulerTimeType.Stride

The interval by which run loop times advance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Stride
```

## Topics

### Creating Scheduler Time Strides

init(TimeInterval)

Creates a run loop scheduler time interval from the given time interval.

### Inspecting Stride Properties

var magnitude: TimeInterval

The value of this time interval in seconds.

var timeInterval: TimeInterval

The value of this time interval in seconds.

## Relationships

### Conforms To

- AdditiveArithmetic
- Comparable
- Decodable
- Encodable
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Numeric
- SchedulerTimeIntervalConvertible
- Sendable
- SignedNumeric

## See Also

### Working with Scheduler Time Intervals

func advanced(by: RunLoop.SchedulerTimeType.Stride) -> RunLoop.SchedulerTimeType

Returns a run loop scheduler time calculated by advancing this instance’s time by the given interval.

func distance(to: RunLoop.SchedulerTimeType) -> RunLoop.SchedulerTimeType.Stride

Returns the distance to another run loop scheduler time.

