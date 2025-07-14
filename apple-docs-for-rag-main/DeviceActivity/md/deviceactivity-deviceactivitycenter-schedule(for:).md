

- DeviceActivity
- DeviceActivityCenter
-  schedule(for:) 

Instance Method

# schedule(for:)

Fetches the schedule of a device activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func schedule(for activity: DeviceActivityName) -> DeviceActivitySchedule?
```

## Parameters 

`activity`  

The name of the activity.

## Return Value

The schedule of the activity or `nil` if no such activity is currently monitored.

## Discussion

The returned object is a static representation of the schedule at the time the function was called. In other words, a `Schedule` fetched for a particular activity doesn’t dynamically update in response to future changes made to that activity.

## See Also

### Getting the Events and Schedules

func events(for: DeviceActivityName) -> [DeviceActivityEvent.Name : DeviceActivityEvent]

Fetches the events of a device activity.

