

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  stop 

# stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

``` source
virtual void stop(
 IOService *provider ); 
```

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

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

