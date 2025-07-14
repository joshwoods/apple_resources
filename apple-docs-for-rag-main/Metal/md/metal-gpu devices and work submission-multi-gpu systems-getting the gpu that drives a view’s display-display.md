

- Metal
- GPU Devices and Work Submission
- Multi-GPU Systems
-  Getting the GPU that Drives a View’s Display 

Article

# Getting the GPU that Drives a View’s Display

Keep up to date with the optimal device for your display.

## Overview

A user can have multiple external displays connected directly to a Mac or to an external GPU. Each view in your app shows on a single display, and a single GPU drives each display. The display in which your view appears and the GPU that drives the display can change dynamically; therefore, you need to prepare your app to handle these changes. Register for display change notifications, get the device that drives your view’s display, and decide if your app should use that device to present rendered graphics.

### Handle Display Change Notifications

Register for the following notifications so the system can notify your app about specific display changes:

didChangeScreenNotification  
The system posts this notification when any window, including the window containing your view, moves to a different display.

didChangeScreenParametersNotification  
The system posts this notification when the Mac system’s display configuration changes; for example, when the user connects or disconnects an external display from the system. Another example is when the GPU driving the display changes, such as when system has automatic graphics switching enabled and switches between the discrete and integrated GPUs to drive the display.

When the system posts a display change notification, you can decide if you should get and use a new device.

- Swift
- Objective-C

```
@objc func handleDisplayChanges(notification: NSNotification) {
    // Handle display changes
}

func registerForDisplayChangeNotifications() {
    NotificationCenter.default.addObserver(self,
                                           selector: #selector(handleDisplayChanges(notification:)),
                                           name: NSNotification.Name(rawValue: "NSWindowDidChangeScreenNotification"),
                                           object: nil)

    NotificationCenter.default.addObserver(self,
                                           selector: #selector(handleDisplayChanges(notification:)),
                                           name: NSNotification.Name(rawValue: "NSApplicationDidChangeScreenParametersNotification"),
                                           object: nil)
}
```

```
- (void)handleDisplayChanges:(NSNotification *)notification
{
    // Handle display changes
}

- (void)registerForDisplayChangeNotifications
{
    [[NSNotificationCenter defaultCenter] addObserver:self
                                             selector:@selector(handleDisplayChanges:)
                                                 name:NSWindowDidChangeScreenNotification
                                               object:nil];

    [[NSNotificationCenter defaultCenter] addObserver:self
                                             selector:@selector(handleDisplayChanges:)
                                                 name:NSApplicationDidChangeScreenParametersNotification
                                               object:nil];
}
```

To deregister from the previous notifications, call the removeObserver(_:name:object:) method.

### Identify the Device that Drives Your View’s Display

Get the CGDirectDisplayID value for the display in which your view currently appears. Then call the CGDirectDisplayCopyCurrentMetalDevice(_:) function to get the device that drives that display.

- Swift
- Objective-C

```
guard let viewDisplayID = mtkView.window?.screen?.deviceDescription[NSDeviceDescriptionKey("NSScreenNumber")] as? CGDirectDisplayID else { return }
let displayDevice = CGDirectDisplayCopyCurrentMetalDevice(viewDisplayID)
```

```
NSNumber           *screenNumber = _mtkView.window.screen.deviceDescription[@"NSScreenNumber"];
CGDirectDisplayID  viewDisplayID  = [screenNumber unsignedIntValue];
id      displayDevice  = CGDirectDisplayCopyCurrentMetalDevice(viewDisplayID);
```

## See Also

### Locating GPUs

Finding Multiple GPUs on an Intel-based Mac

Locate, identify, and choose suitable GPUs for your app.

func MTLCopyAllDevices() -> [any MTLDevice]

Returns an array of all the Metal device instances in the system.

func MTLCopyAllDevicesWithObserver(handler: MTLDeviceNotificationHandler) -> (devices: [any MTLDevice], observer: NSObject)

Returns an array of all the Metal GPU devices in the system and registers a notification handler that Metal calls when the device list changes.

func MTLRemoveDeviceObserver(any NSObjectProtocol)

Removes a registered observer of device notifications.

func CGDirectDisplayCopyCurrentMetalDevice(_ display: CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

typealias MTLDeviceNotificationHandler

A Swift closure or an Objective-C block that Metal calls when the system adds or removes a GPU device.

struct MTLDeviceNotificationName

A notification that represents a change to a GPU device in the system.

