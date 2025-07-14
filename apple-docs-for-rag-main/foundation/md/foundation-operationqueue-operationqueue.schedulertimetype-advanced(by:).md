

- Foundation
- OperationQueue
- OperationQueue.SchedulerTimeType
-  advanced(by:) 

Instance Method

# advanced(by:)

Calculates an operation queue scheduler time by advancing the scheduler time type’s date by the given interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func advanced(by n: OperationQueue.SchedulerTimeType.Stride) -> OperationQueue.SchedulerTimeType
```

## Parameters 

`n`  

The time interval to advance date by.

## Return Value

An operation queue scheduler time advanced by the given interval from date.

## See Also

### Managing Scheduler Time Type Properties

var date: Date

The date this type represents.

func distance(to: OperationQueue.SchedulerTimeType) -> OperationQueue.SchedulerTimeType.Stride

The distance to another operation queue scheduler time.

struct Stride

The interval by which operation queue times advance.

