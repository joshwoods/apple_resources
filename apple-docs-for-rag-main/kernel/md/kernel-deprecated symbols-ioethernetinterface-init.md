

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  init 

# init

Initializes an IOEthernetInterface instance.

``` source
virtual bool init(
 IONetworkController *controller ); 
```

## Parameters 

`controller`  

A network controller object that will service the interface object being initialized.

## Return Value

Returns true on success, false otherwise.

## Overview

Instance variables are initialized, and an arpcom structure is allocated.

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

performCommand

Handles an ioctl command sent to the Ethernet interface.

