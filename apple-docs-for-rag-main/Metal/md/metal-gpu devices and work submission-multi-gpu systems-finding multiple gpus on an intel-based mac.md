

- Metal
- GPU Devices and Work Submission
- Multi-GPU Systems
-  Finding Multiple GPUs on an Intel-based Mac 

Article

# Finding Multiple GPUs on an Intel-based Mac

Locate, identify, and choose suitable GPUs for your app.

## Overview

Your app can use multiple GPUs on an Intel-based Mac, including any built-in and external GPUs. Start by getting a list of all the system’s available GPUs, and then submit workloads to those appropriate for your app’s tasks.

Note

Mac computers with Apple silicon have a single, high-performance, and energy-efficient GPU.

### Get a List of GPU Devices

Your app can get an array of MTLDevice instances, each of which represents an available GPU, by calling the MTLCopyAllDevices() function.

- Swift
- Objective-C

```
let devices = MTLCopyAllDevices()
```

```
NSArray> *devices = MTLCopyAllDevices();
```

However, that function provides a list of GPUs that are available at that moment in time. To get the current list and register for device update notifications, provide a handler to Metal by calling the MTLCopyAllDevicesWithObserver function.

- Swift
- Objective-C

```
let (devices, observer) = MTLCopyAllDevicesWithObserver() { (device, notification) in
    self.device(device, issued: notification)
}
```

```
id deviceObserver = nil;
NSArray> *devices = nil;

devices = MTLCopyAllDevicesWithObserver(&deviceObserver,
                                        ^(id device,
                                          MTLDeviceNotificationName name) {
    [self device:device hasNotification:name];
});
```

Metal calls your handler to tell your app when the system adds or removes an MTLDevice from the system.

Note

Metal calls your app’s handler when a device may change its state in the future, such as when a person makes a safe disconnect request. For more information, see Handling External GPU Additions and Removals.

Your app can deregister its observer when it no longer needs GPU device updates from the system by calling the MTLRemoveDeviceObserver(_:) function.

- Swift
- Objective-C

```
MTLRemoveDeviceObserver(observer)
```

```
MTLRemoveDeviceObserver(deviceObserver);
```

### Identify Each GPU by Type

Each GPU on a Mac computer’s system can be one of three types: integrated, discrete, or external. You can identify each MTLDevice instance’s type by inspecting its isLowPower and isRemovable properties.

| GPU Type | isLowPower | isRemovable |
|----|----|----|
| Integrated | true | false |
| Discrete | false | false |
| External | false | true |

For example, you can use these properties to build a list of devices for each GPU type.

- Swift
- Objective-C

```
var externalGPUs = [MTLDevice]()
var discreteGPUs = [MTLDevice]()
var integratedGPUs = [MTLDevice]()

for device in devices {
    if device.isRemovable { externalGPUs.append(device) } else
    if device.isLowPower { integratedGPUs.append(device) } else {
        discreteGPUs.append(device)
    }
}
```

```
NSMutableArray> *externalGPUs = [[NSMutableArray alloc] init];
NSMutableArray> *discreteGPUs = [[NSMutableArray alloc] init];
NSMutableArray> *integratedGPUs = [[NSMutableArray alloc] init];

for (id device in devices) {
    if (device.isRemovable) { [externalGPUs addObject:device]; }
    else if (device.isLowPower) { [integratedGPUs addObject:device]; }
    else { [discreteGPUs addObject:device]; }
}
```

Some external or discrete GPUs can also be *headless*, which means they aren’t connected to a display. Your app can identify whether a GPU is headless by checking a device instance’s isHeadless property.

- Swift
- Objective-C

```
if device.isHeadless {
    // This GPU device isn't connected to any displays.
    ...
}
```

```
if (device.isHeadless) {
    // This GPU device isn't connected to any displays.
    ...
}
```

### Select the GPUs Suitable for Your Workloads

Each GPU type has its advantages for certain tasks or workloads that you can consider for a system with multiple GPUs.

| GPU type   | Power consumption | Memory bandwidth |
|------------|-------------------|------------------|
| Integrated | Low               | High             |
| Discrete   | Medium            | High             |
| External   | High              | Low              |

In general, start with an integrated GPU (if the system has one) to conserve power and extend the device’s battery life. If your app needs additional graphics or compute processing, consider moving some workloads to a discrete GPU, if the system has one.

Tip

Your app could let a person choose which GPU your app uses for its workloads, especially if they attach an external GPU to their system.

External GPUs typically have significant processing power but lower bandwidth compared to internal GPUs, which makes them a good choice for tasks that don’t require much memory bandwidth for each frame, including the following:

- Rendering high-complexity graphics scenes

- Rendering high-resolution graphics content

- Processing compute workloads in tandem with rendering graphics

- Processing compute workloads that use a high arithmetic-logic unit (ALU) complexity

For more information about GPU memory bandwidth, see Adjusting for GPU Memory Bandwidth Tradeoffs.

Note

A headless GPU is more suitable for compute processing than rendering graphics for a display because the GPU isn’t connected to a display.

## See Also

### Locating GPUs

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

typealias MTLDeviceNotificationHandler

A Swift closure or an Objective-C block that Metal calls when the system adds or removes a GPU device.

struct MTLDeviceNotificationName

A notification that represents a change to a GPU device in the system.

