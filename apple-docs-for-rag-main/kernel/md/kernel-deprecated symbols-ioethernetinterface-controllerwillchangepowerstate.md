

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  controllerWillChangePowerState 

# controllerWillChangePowerState

Handles a notification that the network controller servicing this interface object is about to transition to a new power state.

``` source
virtual IOReturn controllerWillChangePowerState( 
 IONetworkController *controller, 
 IOPMPowerFlagsflags, 
 UInt32stateNumber, 
 IOService *policyMaker); 
```

## Parameters 

`controller`  

The network controller object.

`flags`  

Flags that describe the capability of the controller in the new power state.

`stateNumber`  

An index to a state in the network controller's power state array that the controller is switching to.

`policyMaker`  

A reference to the network controller's policy-maker, and is also the originator of this notification.

## Return Value

Always returns kIOReturnSuccess.

## Overview

If the controller is about to transition to an unusable state, and it is currently enabled, then the disable() method on the controller is called.

## See Also

### Miscellaneous

controllerDidChangePowerState

Handles a notification that the network controller servicing this interface object has transitioned to a new power state.

controllerDidOpen

A notification that the interface has opened the network controller.

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

