

- Metal
- MTLDeviceNotificationName
-  removalRequested 

Type Property

# removalRequested

A notification that Metal sends to observers when a person requests to remove a GPU device from the system.

macOS 10.13+

``` source
static let removalRequested: MTLDeviceNotificationName
```

## Mentioned in 

Handling External GPU Additions and Removals

## Discussion

This notification tells your app to stop using an MTLDevice instance by releasing any objects and resources your app created with it.

Note

Metal removes the device instance from the array it returns with its methods — such as MTLCopyAllDevices() — before sending this notification.

## See Also

### Creating a notification name

static let wasAdded: MTLDeviceNotificationName

A notification that Metal sends to observers when the system adds a GPU device.

static let wasRemoved: MTLDeviceNotificationName

A notification that Metal sends to observers when the system removes a GPU device.

init(rawValue: String)

Creates a Metal device notification name from a string.

