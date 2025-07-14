

- IOUSBHost
- IOUSBHostObjectInitOptions
-  deviceCapture 

Type Property

# deviceCapture

The option to capture the device and terminate existing drivers.

Mac Catalyst 14.0+macOS 10.15+

``` source
static var deviceCapture: IOUSBHostObjectInitOptions { get }
```

## Discussion

Callers must have either the com.apple.vm.device-access entitlement and the IOUSBHostDevice object from IOServiceAuthorize(_:_:) authorization, or have root privileges. Using this option terminates all clients and drivers of the IOUSBHostDevice and associated IOUSBHostInterface clients, as well as the caller. Upon destroy() of the IOUSBHostDevice, the device resets and IOUSBHostInterface reregisters for IOKit matching.

