

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  handleIsOpen 

# handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

``` source
virtual bool handleIsOpen(
 const IOService *forClient ) const; 
```

## Parameters 

`forClient`  

If non-zero, isOpen returns the open state for that client. If zero is passed, isOpen returns the open state for all clients.

## Return Value

Returns true if the specific, or any, client has the IOService open.

## Overview

See IOService for discussion.

## See Also

### Miscellaneous

getFireWireUnit

Returns an IOFireWireUnit object.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

