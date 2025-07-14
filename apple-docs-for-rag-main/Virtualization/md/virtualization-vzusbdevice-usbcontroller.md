

- Virtualization
- VZUSBDevice
-  usbController 

Instance Property

# usbController

The USB controller that has an attachment to the device.

macOS 15.0+

``` source
weak var usbController: VZUSBController? { get }
```

**Required**

## Discussion

If a USB device object that conforms to this protocol has a current attachment to a USB controller, this property includes a pointer to the device’s USB controller object. Otherwise, it’s `nil`.

## See Also

### Properties

var uuid: UUID

The device’s unique identifier.

**Required**

