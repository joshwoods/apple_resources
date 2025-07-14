

- Virtualization
- VZUSBController
-  usbDevices 

Instance Property

# usbDevices

The list of attached USB devices for the controller.

macOS 15.0+

``` source
var usbDevices: [any VZUSBDevice] { get }
```

## Discussion

If a VZVirtualMachineConfiguration contains a USB controller configuration that contains USB devices, those devices appear in the list when you start the virtual machine.

## See Also

### Related Documentation

protocol VZUSBDevice

A protocol that represents a USB device in a VM.

protocol VZUSBDeviceConfiguration

The protocol for configuring USB devices.

class VZUSBControllerConfiguration

The base class for a USB controller configuration.

