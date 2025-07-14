

- Metal
-  MTLDeviceNotificationHandler 

Type Alias

# MTLDeviceNotificationHandler

A Swift closure or an Objective-C block that Metal calls when the system adds or removes a GPU device.

macOS 10.13+

``` source
typealias MTLDeviceNotificationHandler = (any MTLDevice, MTLDeviceNotificationName) -> Void
```

## Parameters 

`device`  

A MTLDevice that represents the GPU that’s sending the notification.

`notifyName`  

A notification that represents a change to a GPU device in the system.

## See Also

### Locating GPUs

Finding Multiple GPUs on an Intel-based Mac

Locate, identify, and choose suitable GPUs for your app.

Getting the GPU that Drives a View’s Display

Keep up to date with the optimal device for your display.

func MTLCopyAllDevices() -> [any MTLDevice]

Returns an array of all the Metal device instances in the system.

func MTLCopyAllDevicesWithObserver(handler: MTLDeviceNotificationHandler) -> (devices: [any MTLDevice], observer: NSObject)

Returns an array of all the Metal GPU devices in the system and registers a notification handler that Metal calls when the device list changes.

func MTLRemoveDeviceObserver(any NSObjectProtocol)

Removes a registered observer of device notifications.

func CGDirectDisplayCopyCurrentMetalDevice(_ display: CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

struct MTLDeviceNotificationName

A notification that represents a change to a GPU device in the system.

