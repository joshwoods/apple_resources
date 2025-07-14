

- Virtualization
-  VZUSBController 

Class

# VZUSBController

A class that represents a USB controller in a VM.

macOS 15.0+

``` source
class VZUSBController
```

## Overview

Don’t create a `VZUSBController` directly. You need to first configure USB controllers on a VZVirtualMachineConfiguration through a subclass of VZUSBControllerConfiguration. When you create a VZVirtualMachine from the configuration, the USB controllers are available through the usbControllers property.

The concrete type of a `VZUSBController` corresponds to the type the configuration uses. For example, a VZXHCIControllerConfiguration leads to a device of type VZXHCIController.

## Topics

### Instance properties

var usbDevices: [any VZUSBDevice]

The list of attached USB devices for the controller.

### Attaching and detaching devices

func attach(device: any VZUSBDevice, completionHandler: ((any Error)?) -> Void)

Attaches a USB device to the controller.

func detach(device: any VZUSBDevice, completionHandler: ((any Error)?) -> Void)

Detaches a USB device from the controller.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZXHCIController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Controllers

class VZXHCIController

A class that represents a USB Extensible Host Controller Interface (XHCI) controller in a VM.

