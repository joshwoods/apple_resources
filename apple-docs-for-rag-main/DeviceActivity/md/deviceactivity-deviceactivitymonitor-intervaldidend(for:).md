

- DeviceActivity
- DeviceActivityMonitor
-  intervalDidEnd(for:) 

Instance Method

# intervalDidEnd(for:)

Indicates that the device activity interval ended.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func intervalDidEnd(for activity: DeviceActivityName)
```

## Parameters 

`activity`  

The name of the activity.

## Discussion

An activity ends when someone first uses the device outside the activity’s scheduled time interval or when your app stops monitoring an activity with an ongoing interval. In other words, the system only invokes this method when the device is in use.

## See Also

### Monitoring Scheduled Intervals

func intervalDidStart(for: DeviceActivityName)

Indicates that the device activity interval started.

func intervalWillEndWarning(for: DeviceActivityName)

Warns your app of an ongoing activity’s conclusion a specified time before the activity ends.

func intervalWillStartWarning(for: DeviceActivityName)

Warns your app of an upcoming activity a specified time before the activity starts.

