

- Virtualization
- VZUSBDevice
-  uuid 

Instance Property

# uuid

The device’s unique identifier.

macOS 15.0+

``` source
var uuid: UUID { get }
```

**Required**

## Discussion

This is the identifier the system creates from device configuration objects that conform to VZUSBDeviceConfiguration.

## See Also

### Properties

var usbController: VZUSBController?

The USB controller that has an attachment to the device.

**Required**

