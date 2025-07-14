

- DeviceActivity
- DeviceActivityCenter
-  events(for:) 

Instance Method

# events(for:)

Fetches the events of a device activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func events(for activity: DeviceActivityName) -> [DeviceActivityEvent.Name : DeviceActivityEvent]
```

## Parameters 

`activity`  

The name of the activity.

## Return Value

The events of the activity. The dictionary is empty if your app doesn’t monitor the activity.

## Discussion

The returned object is a static representation of the events at the time the function was called. In other words, an `Event` fetched for a particular activity doesn’t dynamically update in response to future changes made to that activity.

## See Also

### Getting the Events and Schedules

func schedule(for: DeviceActivityName) -> DeviceActivitySchedule?

Fetches the schedule of a device activity.

