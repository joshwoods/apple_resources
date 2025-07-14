

- Foundation
- OperationQueue
- OperationQueue.SchedulerTimeType
-  distance(to:) 

Instance Method

# distance(to:)

The distance to another operation queue scheduler time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func distance(to other: OperationQueue.SchedulerTimeType) -> OperationQueue.SchedulerTimeType.Stride
```

## Parameters 

`other`  

Another operation queue scheduler time.

## Return Value

The time interval between this time and the other time.

## See Also

### Managing Scheduler Time Type Properties

var date: Date

The date this type represents.

func advanced(by: OperationQueue.SchedulerTimeType.Stride) -> OperationQueue.SchedulerTimeType

Calculates an operation queue scheduler time by advancing the scheduler time type’s date by the given interval.

struct Stride

The interval by which operation queue times advance.

