

- DeviceActivity
- DeviceActivityCenter
-  stopMonitoring(\_:) 

Instance Method

# stopMonitoring(\_:)

Stops monitoring the specified device activities.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func stopMonitoring(_ activities: [DeviceActivityName] = [])
```

## Parameters 

`activities`  

The names of the activities. If the array is empty or no `activities` are explicitly specified, this method stops monitoring all activities.

## Discussion

This method ignores names that don’t correspond to monitored activities.

## See Also

### Monitoring Device Activities

init()

Creates an activity center to manage which device activities your application monitors.

func startMonitoring(DeviceActivityName, during: DeviceActivitySchedule, events: [DeviceActivityEvent.Name : DeviceActivityEvent]) throws

Starts monitoring the specified device activity.

var activities: [DeviceActivityName]

The activities that the application’s extension currently monitors.

