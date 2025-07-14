

- Metal
-  MTLCopyAllDevicesWithObserver(handler:) 

Function

# MTLCopyAllDevicesWithObserver(handler:)

Returns an array of all the Metal GPU devices in the system and registers a notification handler that Metal calls when the device list changes.

macOS 10.13+Swift 4.0+

``` source
func MTLCopyAllDevicesWithObserver(handler: @escaping MTLDeviceNotificationHandler) -> (devices: [any MTLDevice], observer: NSObject)
```

## Parameters 

`handler`  

A notification handler you implement that Metal calls when the system adds or removes a GPU device from the system.

## Return Value

`devices`  
An array of MTLDevice instances

`observer`  
An object instance that represents an observer the function creates for you.

## Discussion

Keep a copy of `observer` in your app in case you want to stop receiving notifications. You can stop receiving notifications by passing `observer` to the MTLRemoveDeviceObserver(_:) function.

## See Also

### Locating GPUs

Finding Multiple GPUs on an Intel-based Mac

Locate, identify, and choose suitable GPUs for your app.

Getting the GPU that Drives a View’s Display

Keep up to date with the optimal device for your display.

func MTLCopyAllDevices() -> [any MTLDevice]

Returns an array of all the Metal device instances in the system.

func MTLRemoveDeviceObserver(any NSObjectProtocol)

Removes a registered observer of device notifications.

func CGDirectDisplayCopyCurrentMetalDevice(_ display: CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

typealias MTLDeviceNotificationHandler

A Swift closure or an Objective-C block that Metal calls when the system adds or removes a GPU device.

struct MTLDeviceNotificationName

A notification that represents a change to a GPU device in the system.

