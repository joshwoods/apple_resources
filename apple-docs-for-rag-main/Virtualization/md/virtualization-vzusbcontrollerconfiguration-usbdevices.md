

- Virtualization
- VZUSBControllerConfiguration
-  usbDevices 

Instance Property

# usbDevices

The list of USB devices.

macOS 15.0+

``` source
var usbDevices: [any VZUSBDeviceConfiguration] { get set }
```

## Discussion

This list represents a set of USB devices that a VM starts with. For each entry in the list, the system creates a corresponding runtime object in the usbDevices property.

The list is empty by default.

## See Also

### Related Documentation

class VZUSBController

A class that represents a USB controller in a VM.

protocol VZUSBDeviceConfiguration

The protocol for configuring USB devices.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

