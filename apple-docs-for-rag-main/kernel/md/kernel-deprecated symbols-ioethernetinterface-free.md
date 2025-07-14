

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  free 

# free

Frees the IOEthernetInterface instance.

``` source
virtual void free(); 
```

## Overview

The memory allocated for the arpcom structure is released, followed by a call to super::free().

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

getNamePrefix

Returns a string containing the prefix to use when creating a BSD name for this interface.

init

Initializes an IOEthernetInterface instance.

performCommand

Handles an ioctl command sent to the Ethernet interface.

