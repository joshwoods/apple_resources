

- DeviceActivity
- DeviceActivityCenter
-  activities 

Instance Property

# activities

The activities that the application’s extension currently monitors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var activities: [DeviceActivityName] { get }
```

## See Also

### Monitoring Device Activities

init()

Creates an activity center to manage which device activities your application monitors.

func startMonitoring(DeviceActivityName, during: DeviceActivitySchedule, events: [DeviceActivityEvent.Name : DeviceActivityEvent]) throws

Starts monitoring the specified device activity.

func stopMonitoring([DeviceActivityName])

Stops monitoring the specified device activities.

