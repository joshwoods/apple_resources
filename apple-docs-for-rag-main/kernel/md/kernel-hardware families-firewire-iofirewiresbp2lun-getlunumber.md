

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  getLUNumber 

# getLUNumber

Returns the LUNs number.

``` source
virtual UInt32 getLUNumber(
 void ); 
```

## Return Value

Returns a UInt32 containing the Logical Unit Number.

## Overview

Each LUN has a number to uniquely identify it on a device. This method returns this value in a UInt32.

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

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

