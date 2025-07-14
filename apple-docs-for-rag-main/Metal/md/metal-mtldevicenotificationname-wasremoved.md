

- Metal
- MTLDeviceNotificationName
-  wasRemoved 

Type Property

# wasRemoved

A notification that Metal sends to observers when the system removes a GPU device.

macOS 10.13+

``` source
static let wasRemoved: MTLDeviceNotificationName
```

## Mentioned in 

Handling External GPU Additions and Removals

## Discussion

This notification tells your app that an MTLDevice instance and its methods are no longer valid to avoid runtime failures.

Important

If a person removes a GPU without warning, this notification may be posted without a prior removalRequested notification.

## See Also

### Creating a notification name

static let wasAdded: MTLDeviceNotificationName

A notification that Metal sends to observers when the system adds a GPU device.

static let removalRequested: MTLDeviceNotificationName

A notification that Metal sends to observers when a person requests to remove a GPU device from the system.

init(rawValue: String)

Creates a Metal device notification name from a string.

