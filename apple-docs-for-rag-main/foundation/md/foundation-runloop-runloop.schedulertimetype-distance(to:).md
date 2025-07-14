

- Foundation
- RunLoop
- RunLoop.SchedulerTimeType
-  distance(to:) 

Instance Method

# distance(to:)

Returns the distance to another run loop scheduler time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func distance(to other: RunLoop.SchedulerTimeType) -> RunLoop.SchedulerTimeType.Stride
```

## Parameters 

`other`  

Another run loop time.

## Return Value

The time interval between this time and the provided time.

## See Also

### Working with Scheduler Time Intervals

struct Stride

The interval by which run loop times advance.

func advanced(by: RunLoop.SchedulerTimeType.Stride) -> RunLoop.SchedulerTimeType

Returns a run loop scheduler time calculated by advancing this instance’s time by the given interval.

