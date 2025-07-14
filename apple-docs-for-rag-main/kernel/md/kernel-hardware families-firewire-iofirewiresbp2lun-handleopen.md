

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
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

attach

Attaches an IOService client to a provider in the registry.

createLogin

Creates a new IOFireWireSBP2Login object.

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

matchPropertyTable

Implements SBP2 specific matching.

