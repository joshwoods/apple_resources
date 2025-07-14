

- DeviceActivity
- DeviceActivityMonitor
-  intervalWillEndWarning(for:) 

Instance Method

# intervalWillEndWarning(for:)

Warns your app of an ongoing activity’s conclusion a specified time before the activity ends.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func intervalWillEndWarning(for activity: DeviceActivityName)
```

## Parameters 

`activity`  

The name of the activity.

## Discussion

When an activity is about to end, `intervalWillEndWarning` warns your app extension of the concluding activity.

## See Also

### Monitoring Scheduled Intervals

func intervalDidEnd(for: DeviceActivityName)

Indicates that the device activity interval ended.

func intervalDidStart(for: DeviceActivityName)

Indicates that the device activity interval started.

func intervalWillStartWarning(for: DeviceActivityName)

Warns your app of an upcoming activity a specified time before the activity starts.

