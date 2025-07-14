

- Dispatch
- DispatchSourceTimer
-  scheduleRepeating(wallDeadline:interval:leeway:) Deprecated

Instance Method

# scheduleRepeating(wallDeadline:interval:leeway:)

Schedules a repeating timer with the specified time, repeat interval, and leeway values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwiftDeprecated

``` source
func scheduleRepeating(
    wallDeadline: DispatchWallTime,
    interval: DispatchTimeInterval,
    leeway: DispatchTimeInterval = .nanoseconds(0)
)
```

Deprecated

Use schedule(wallDeadline:repeating:leeway:) instead.

## Parameters 

`wallDeadline`  

The time at which to execute the dispatch source’s event handler.

`interval`  

The repeat interval for the timer, measured in seconds.

`leeway`  

The maximum amount of time after `wallDeadline` by which the system may delay the delivery of the timer event.

## Discussion

The system may defer the deliver of timer events to improve power consumption and system performance. The first time the timer fires, the maximum allowable delay is equal to the value in the `leeway` parameter. For subsequent firings, the timer fires at `wallDeadline + (n * repeating)`, and the maximum delay is equal to `min(leeway, repeating/2)`—that is, the smaller of either the `leeway` value or half the value in the `repeating` parameter.

The system may fire a timer sooner than the value in the `wallDeadline` parameter. If you created the timer with the strict flag, the system makes every effort to observe the provided `leeway` value, even if it is smaller than the current lower limit.

Calling this method on a cancelled dispatch source has no effect.

## See Also

### Deprecated

func scheduleOneshot(deadline: DispatchTime, leeway: DispatchTimeInterval)

Schedules a timer to fire once with the specified deadline and leeway values.

Deprecated

func scheduleOneshot(wallDeadline: DispatchWallTime, leeway: DispatchTimeInterval)

Schedules a timer to fire once with the specified deadline and leeway values.

Deprecated

func scheduleRepeating(deadline: DispatchTime, interval: DispatchTimeInterval, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified deadline, repeat interval, and leeway values.

Deprecated

func scheduleRepeating(deadline: DispatchTime, interval: Double, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified deadline, repeat interval, and leeway values.

Deprecated

func scheduleRepeating(wallDeadline: DispatchWallTime, interval: Double, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified time, repeat interval, and leeway values.

Deprecated

