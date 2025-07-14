

- Foundation
- OperationQueue
-  OperationQueue.SchedulerTimeType 

Structure

# OperationQueue.SchedulerTimeType

The scheduler time type the operation queue uses.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SchedulerTimeType
```

## Topics

### Creating Scheduler Time Types

init(Date)

Creates an operation queue scheduler time with the given date.

### Managing Scheduler Time Type Properties

var date: Date

The date this type represents.

func advanced(by: OperationQueue.SchedulerTimeType.Stride) -> OperationQueue.SchedulerTimeType

Calculates an operation queue scheduler time by advancing the scheduler time type’s date by the given interval.

func distance(to: OperationQueue.SchedulerTimeType) -> OperationQueue.SchedulerTimeType.Stride

The distance to another operation queue scheduler time.

struct Stride

The interval by which operation queue times advance.

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

### Scheduling Operations

struct SchedulerOptions

A type that defines options the operation queue accepts.

