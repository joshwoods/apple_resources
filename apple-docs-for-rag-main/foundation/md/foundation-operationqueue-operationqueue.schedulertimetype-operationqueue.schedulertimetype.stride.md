

- Foundation
- OperationQueue
- OperationQueue.SchedulerTimeType
-  OperationQueue.SchedulerTimeType.Stride 

Structure

# OperationQueue.SchedulerTimeType.Stride

The interval by which operation queue times advance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Stride
```

## Topics

### Managing Stride Properties

var timeInterval: TimeInterval

The value of this time interval, in seconds.

var magnitude: TimeInterval

The value of this time interval, in seconds.

### Creating Scheduler Time Strides

init(TimeInterval)

Creates a stride using the specified time interval.

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

### Managing Scheduler Time Type Properties

var date: Date

The date this type represents.

func advanced(by: OperationQueue.SchedulerTimeType.Stride) -> OperationQueue.SchedulerTimeType

Calculates an operation queue scheduler time by advancing the scheduler time type’s date by the given interval.

func distance(to: OperationQueue.SchedulerTimeType) -> OperationQueue.SchedulerTimeType.Stride

The distance to another operation queue scheduler time.

