

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  controllerDidOpen 

# controllerDidOpen

A notification that the interface has opened the network controller.

``` source
virtual bool controllerDidOpen(
 IONetworkController *controller); 
```

## Parameters 

`controller`  

The controller object that was opened.

## Return Value

Returns true on success, false otherwise. Returning false will cause the controller to be closed, and any pending client opens to be rejected.

## Overview

This method will be called by IONetworkInterface after a network controller has accepted an open from this interface object. IOEthernetInterface will first call the implementation in its superclass, then inspect the controller through properties published in the registry. This method is called with the arbitration lock held.

## See Also

### Miscellaneous

controllerDidChangePowerState

Handles a notification that the network controller servicing this interface object has transitioned to a new power state.

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

