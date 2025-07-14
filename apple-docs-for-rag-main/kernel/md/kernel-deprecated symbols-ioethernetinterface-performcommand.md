

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  performCommand 

# performCommand

Handles an ioctl command sent to the Ethernet interface.

``` source
virtual SInt32 performCommand(
 IONetworkController *controller, 
 unsigned longcmd, 
 void *arg0, 
 void *arg1); 
```

## Parameters 

`controller`  

The controller object.

`cmd`  

The ioctl command code.

`arg0`  

Command argument 0. Generally a pointer to an ifnet structure associated with the interface.

`arg1`  

Command argument 1.

## Return Value

Returns a BSD return value defined in bsd/sys/errno.h.

## Overview

This method handles socket ioctl commands sent to the Ethernet interface from DLIL. Commands recognized and processed by this method are SIOCSIFADDR, SIOCSIFFLAGS, SIOCADDMULTI, and SIOCDELMULTI. Other commands are passed to the superclass.

## See Also

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

