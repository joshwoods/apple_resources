

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
-  distance(to:) 

Instance Method

# distance(to:)

Returns the distance to another immediate scheduler time; this distance is always `0` in the context of an immediate scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func distance(to other: ImmediateScheduler.SchedulerTimeType) -> ImmediateScheduler.SchedulerTimeType.Stride
```

## Parameters 

`other`  

The other scheduler time.

## Return Value

`0`, as a `Stride`.

## See Also

### Calculating Time Offsets

func advanced(by: ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType

Advances the time by the specified amount; this is meaningless in the context of an immediate scheduler.

