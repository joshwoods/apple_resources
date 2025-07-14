

- DeviceActivity
- DeviceActivityMonitor
-  eventWillReachThresholdWarning(\_:activity:) 

Instance Method

# eventWillReachThresholdWarning(\_:activity:)

Warns your app that an activity is about to reach its threshold.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func eventWillReachThresholdWarning(
    _ event: DeviceActivityEvent.Name,
    activity: DeviceActivityName
)
```

## Parameters 

`event`  

The name of the event.

`activity`  

The name of the activity.

## Discussion

When an activity is about to reach its threshold, `eventWillReachThresholdWarning` warns your app extension of the concluding threshold limit.

## See Also

### Monitoring Event Thresholds

func eventDidReachThreshold(DeviceActivityEvent.Name, activity: DeviceActivityName)

Indicates that the activity reached its threshold.

