

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  createLogin 

# createLogin

Creates a new IOFireWireSBP2Login object.

``` source
virtual IOFireWireSBP2Login *createLogin(
 void ); 
```

## Return Value

Returns a pointer to a new IOFireWireSBP2Login.

## Overview

Creates a new IOFireWireSBP2Login object for the LUN. Login objects supply most of the SBP2 APIs related to login maintenance and Normal Command ORB execution.

## See Also

### Miscellaneous

attach

Attaches an IOService client to a provider in the registry.

createManagementORB

Creates a new IOFireWireSBP2ManagementORB object.

getDiagnostics

Debug-only method.

getFireWireUnit

Returns an IOFireWireUnit object.

getLUNumber

Returns the LUNs number.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

