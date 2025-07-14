

- Metal
- MTLDeviceNotificationName
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a Metal device notification name from a string.

macOS 10.13+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

A string of the notification’s name.

## Discussion

Use this type’s static properties instead of this initializer.

## See Also

### Creating a notification name

static let wasAdded: MTLDeviceNotificationName

A notification that Metal sends to observers when the system adds a GPU device.

static let removalRequested: MTLDeviceNotificationName

A notification that Metal sends to observers when a person requests to remove a GPU device from the system.

static let wasRemoved: MTLDeviceNotificationName

A notification that Metal sends to observers when the system removes a GPU device.

