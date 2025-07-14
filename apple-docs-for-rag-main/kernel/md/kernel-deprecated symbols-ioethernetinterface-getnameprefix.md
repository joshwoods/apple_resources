

- Kernel
- Deprecated Symbols
- IOEthernetInterface
-  getNamePrefix 

# getNamePrefix

Returns a string containing the prefix to use when creating a BSD name for this interface.

``` source
virtual const char * getNamePrefix() const; 
```

## Return Value

Returns a pointer to a constant C string "en". Therefore, Ethernet interfaces will be registered with BSD as en0, en1, etc.

## Overview

The BSD name for each interface object is created by concatenating a string returned by this method, with an unique unit number assigned by IONetworkStack.

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

init

Initializes an IOEthernetInterface instance.

performCommand

Handles an ioctl command sent to the Ethernet interface.

