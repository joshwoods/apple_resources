

- Foundation
- OperationQueue
- OperationQueue.SchedulerTimeType
-  date 

Instance Property

# date

The date this type represents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var date: Date
```

## See Also

### Managing Scheduler Time Type Properties

func advanced(by: OperationQueue.SchedulerTimeType.Stride) -> OperationQueue.SchedulerTimeType

Calculates an operation queue scheduler time by advancing the scheduler time type’s date by the given interval.

func distance(to: OperationQueue.SchedulerTimeType) -> OperationQueue.SchedulerTimeType.Stride

The distance to another operation queue scheduler time.

struct Stride

The interval by which operation queue times advance.

