

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
-  advanced(by:) 

Instance Method

# advanced(by:)

Advances the time by the specified amount; this is meaningless in the context of an immediate scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func advanced(by n: ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType
```

## Parameters 

`n`  

The amount to advance by. The `ImmediateScheduler` ignores this value.

## Return Value

An empty `SchedulerTimeType`.

## See Also

### Calculating Time Offsets

func distance(to: ImmediateScheduler.SchedulerTimeType) -> ImmediateScheduler.SchedulerTimeType.Stride

Returns the distance to another immediate scheduler time; this distance is always `0` in the context of an immediate scheduler.

