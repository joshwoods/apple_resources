

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  controllerWillClose 

# controllerWillClose

A notification that the interface will close the network controller.

``` source
virtual void controllerWillClose(
 IONetworkController *controller); 
```

## Parameters 

`controller`  

The controller that is about to be closed.

## Overview

This method will simply call super to propagate the method call. This method is called with the arbitration lock held.

## See Also

### Miscellaneous

controllerDidChangePowerState

Handles a notification that the network controller servicing this interface object has transitioned to a new power state.

controllerDidOpen

A notification that the interface has opened the network controller.

controllerWillChangePowerState

Handles a notification that the network controller servicing this interface object is about to transition to a new power state.

free

Frees the IOEthernetInterface instance.

getNamePrefix

Returns a string containing the prefix to use when creating a BSD name for this interface.

init

Initializes an IOEthernetInterface instance.

performCommand

Handles an ioctl command sent to the Ethernet interface.

