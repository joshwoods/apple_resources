

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  handleOpen 

# handleOpen

Overrideable method to control the open / close behaviour of an IOService.

``` source
virtual bool handleOpen(
 IOService *forClient,
 IOOptionBits options,
 void *arg ); 
```

## Parameters 

`forClient`  

Designates the client of the provider requesting the open.

`options`  

Options for the open, may be interpreted by the implementor of handleOpen.

## Return Value

Return true if the open was successful, false otherwise.

## Overview

See IOService for discussion.

## See Also

### Miscellaneous

getFireWireUnit

Returns an IOFireWireUnit object.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

