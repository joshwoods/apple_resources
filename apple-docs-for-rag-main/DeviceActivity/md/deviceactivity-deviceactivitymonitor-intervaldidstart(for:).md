

- DeviceActivity
- DeviceActivityMonitor
-  intervalDidStart(for:) 

Instance Method

# intervalDidStart(for:)

Indicates that the device activity interval started.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func intervalDidStart(for activity: DeviceActivityName)
```

## Parameters 

`activity`  

The name of the activity.

## Discussion

An activity starts when someone first uses the device within the activity’s scheduled time interval. In other words, the system only invokes this method when the device is in use.

## See Also

### Monitoring Scheduled Intervals

func intervalDidEnd(for: DeviceActivityName)

Indicates that the device activity interval ended.

func intervalWillEndWarning(for: DeviceActivityName)

Warns your app of an ongoing activity’s conclusion a specified time before the activity ends.

func intervalWillStartWarning(for: DeviceActivityName)

Warns your app of an upcoming activity a specified time before the activity starts.

