

- Metal
- MTLDeviceNotificationName
-  wasAdded 

Type Property

# wasAdded

A notification that Metal sends to observers when the system adds a GPU device.

macOS 10.13+

``` source
static let wasAdded: MTLDeviceNotificationName
```

## Mentioned in 

Handling External GPU Additions and Removals

## See Also

### Creating a notification name

static let removalRequested: MTLDeviceNotificationName

A notification that Metal sends to observers when a person requests to remove a GPU device from the system.

static let wasRemoved: MTLDeviceNotificationName

A notification that Metal sends to observers when the system removes a GPU device.

init(rawValue: String)

Creates a Metal device notification name from a string.

