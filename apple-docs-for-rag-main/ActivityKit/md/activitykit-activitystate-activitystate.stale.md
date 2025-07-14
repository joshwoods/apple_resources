

- ActivityKit
- ActivityState
-  ActivityState.stale 

Case

# ActivityState.stale

The Live Activity content is out of date and needs an update.

iOS 16.2+iPadOS 16.2+

``` source
case stale
```

## Mentioned in 

Displaying live data with Live Activities

Starting and updating Live Activities with ActivityKit push notifications

## Discussion

The content of a Live Activity may become out of date before you can update it. For example, a person may be in an area without a network connection, causing the Live Activity to not receive updates. To tell people that they are looking at outdated Live Activity content, you can configure a staleDate for your Live Activity. At the specified date, the activityState changes to `stale` and you can update the Live Activity to indicate that its content is out of date.

## See Also

### Live Activity states

case active

The Live Activity is active, visible, and can receive content updates.

case dismissed

The Live Activity ended and is no longer visible because a person or the system removed it.

case ended

The Live Activity is visible, but a person, app, or system ended it, and it won’t update its content anymore.

