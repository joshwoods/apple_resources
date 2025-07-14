

- Virtualization
- VZUSBController
-  attach(device:completionHandler:) 

Instance Method

# attach(device:completionHandler:)

Attaches a USB device to the controller.

macOS 15.0+

``` source
func attach(
    device: any VZUSBDevice,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func attach(device: any VZUSBDevice) async throws
```

## Parameters 

`device`  

The USB device to attach.

`completionHandler`  

A block the framework calls after the device attaches, or on an error. The error parameter that passes to the block is `nil` if attaching is successful. The framework calls the block on a VM’s queue.

## Discussion

If the device successfully attaches to the controller, it appears in the usbDevices property, the framework sets its usbController property to point to the attached USB controller, and the completion handler returns `nil`.

If the device has a previous attachment to the current USB controller, or to another USB controller, the attach function fails with VZError.Code.deviceAlreadyAttached. If the controller can’t initialize the device correctly, the attach function fails with VZError.Code.deviceInitializationFailure.

You need to call this method on the virtual machine’s queue.

## See Also

### Related Documentation

protocol VZUSBDevice

A protocol that represents a USB device in a VM.

### Attaching and detaching devices

func detach(device: any VZUSBDevice, completionHandler: ((any Error)?) -> Void)

Detaches a USB device from the controller.

