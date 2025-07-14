

- DeviceActivity
- DeviceActivityMonitor
-  eventDidReachThreshold(\_:activity:) 

Instance Method

# eventDidReachThreshold(\_:activity:)

Indicates that the activity reached its threshold.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func eventDidReachThreshold(
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

The system invokes this method when use of the `activity` reaches its threshold.

## See Also

### Monitoring Event Thresholds

func eventWillReachThresholdWarning(DeviceActivityEvent.Name, activity: DeviceActivityName)

Warns your app that an activity is about to reach its threshold.

