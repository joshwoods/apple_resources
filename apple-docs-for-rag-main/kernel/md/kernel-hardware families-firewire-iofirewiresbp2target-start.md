

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  start 

# start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

``` source
virtual bool start(
 IOService *provider ); 
```

## Return Value

Return true if the start was successful, false otherwise (which will cause the instance to be detached and usually freed).

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

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

