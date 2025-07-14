

- Foundation
- RunLoop
- RunLoop.SchedulerTimeType
-  advanced(by:) 

Instance Method

# advanced(by:)

Returns a run loop scheduler time calculated by advancing this instance’s time by the given interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func advanced(by n: RunLoop.SchedulerTimeType.Stride) -> RunLoop.SchedulerTimeType
```

## Parameters 

`n`  

A time interval to advance.

## Return Value

A dispatch queue time advanced by the given interval from this instance’s time.

## See Also

### Working with Scheduler Time Intervals

struct Stride

The interval by which run loop times advance.

func distance(to: RunLoop.SchedulerTimeType) -> RunLoop.SchedulerTimeType.Stride

Returns the distance to another run loop scheduler time.

