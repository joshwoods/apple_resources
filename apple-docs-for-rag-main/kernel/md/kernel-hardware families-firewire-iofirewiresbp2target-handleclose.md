

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  handleClose 

# handleClose

Overrideable method to control the open / close behaviour of an IOService.

``` source
virtual void handleClose(
 IOService *forClient,
 IOOptionBitsoptions ); 
```

## Parameters 

`forClient`  

Designates the client of the provider requesting the close.

`options`  

Options for the close, may be interpreted by the implementor of handleOpen.

## Overview

See IOService for discussion.

## See Also

### Miscellaneous

getFireWireUnit

Returns an IOFireWireUnit object.

handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

