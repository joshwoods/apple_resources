

- Kernel
- Deprecated Symbols
-  IOEthernetInterface Deprecated

Class

# IOEthernetInterface

The Ethernet interface object.

macOS 10.6–10.15.4Deprecated

``` source
class IOEthernetInterface : IONetworkInterface
```

## Overview

An Ethernet controller driver, that is a subclass of IOEthernetController, will instantiate an object of this class when the driver calls the attachInterface() method. This interface object will then vend an Ethernet interface to DLIL, and manage the connection between the controller driver and the upper networking layers. Drivers will seldom need to subclass IOEthernetInterface.

## Topics

### Miscellaneous

controllerDidChangePowerState

Handles a notification that the network controller servicing this interface object has transitioned to a new power state.

controllerDidOpen

A notification that the interface has opened the network controller.

controllerWillChangePowerState

Handles a notification that the network controller servicing this interface object is about to transition to a new power state.

controllerWillClose

A notification that the interface will close the network controller.

free

Frees the IOEthernetInterface instance.

getNamePrefix

Returns a string containing the prefix to use when creating a BSD name for this interface.

init

Initializes an IOEthernetInterface instance.

performCommand

Handles an ioctl command sent to the Ethernet interface.

### Instance Variables

_reserved

### Instance Methods

- attachToDataLinkLayer

- controllerDidChangePowerState

- controllerDidOpen

- controllerWillChangePowerState

- controllerWillClose

- disableFilter

- enableController

- enableFilter

- feedPacketInputTap

- feedPacketOutputTap

- free

- getFilters

- getMetaClass

- getNamePrefix

- init

- initIfnetParams

- inputEvent

- performCommand

- reportInterfaceWakeFlags

- setFilters

- setupMulticastFilter

- syncSIOCADDMULTI

- syncSIOCDELMULTI

- syncSIOCGIFDEVMTU

- syncSIOCSIFADDR

- syncSIOCSIFCAP

- syncSIOCSIFFLAGS

- syncSIOCSIFLLADDR

- syncSIOCSIFMTU

- willTerminate

### Type Methods

+ enableFilter_Wrapper

+ handleEthernetInputEvent

+ performGatedCommand

## Relationships

### Inherits From

- IONetworkInterface

## See Also

### IOKit

IOUSBDevice

An input/output service object that represents a device on the USB bus.

Deprecated

IOUSBInterface

An object that represents an interface of a device on the USB bus.

Deprecated

IOOFPathMatchingDeprecated

IOUSBHostInterfaceDeprecated

IOUSBHostDeviceDeprecated

IOUSBHostPipeDeprecated

IOUSBHostIOSourceDeprecated

IOUSBHostStreamDeprecated

IOHIDEventDriverDeprecated

IOHIDEventService

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDSystemDeprecated

IOHIKeyboardMapperDeprecated

IOHIKeyboardDeprecated

IOHIPointingDeprecated

IOHIDeviceDeprecated

IOHIDElementDeprecated

IOHIDWorkLoopDeprecated

IOEthernetController

Abstract superclass for Ethernet controllers.

Deprecated

