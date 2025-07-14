

- DeviceActivity
- DeviceActivityCenter
-  init() 

Initializer

# init()

Creates an activity center to manage which device activities your application monitors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init()
```

## Discussion

All instances are equivalent and manage the activities monitored by the application’s extension.

## See Also

### Monitoring Device Activities

func startMonitoring(DeviceActivityName, during: DeviceActivitySchedule, events: [DeviceActivityEvent.Name : DeviceActivityEvent]) throws

Starts monitoring the specified device activity.

func stopMonitoring([DeviceActivityName])

Stops monitoring the specified device activities.

var activities: [DeviceActivityName]

The activities that the application’s extension currently monitors.

