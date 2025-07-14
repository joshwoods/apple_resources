

- Virtualization
- VZUSBController
-  detach(device:completionHandler:) 

Instance Method

# detach(device:completionHandler:)

Detaches a USB device from the controller.

macOS 15.0+

``` source
func detach(
    device: any VZUSBDevice,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func detach(device: any VZUSBDevice) async throws
```

## Parameters 

`device`  

The USB device to detach.

`completionHandler`  

A block the framework calls after the device detaches, or on an error. The error parameter that passes to the block is `nil` if detaching the device is successful. The framework calls the block on a VM’s queue.

## Discussion

If the device successfully detaches from the controller, it disappears from the usbDevices property, the framework sets its usbController property to `nil,` and the completion handler returns `nil`.

If the device doesn’t have an attachment to the controller at the time of calling the detach method, the process fails with VZError.Code.deviceNotFound.

You need to call this method on the virtual machine’s queue.

## See Also

### Related Documentation

protocol VZUSBDevice

A protocol that represents a USB device in a VM.

### Attaching and detaching devices

func attach(device: any VZUSBDevice, completionHandler: ((any Error)?) -> Void)

Attaches a USB device to the controller.

