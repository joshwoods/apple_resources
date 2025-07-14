

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
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

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

