

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  getFireWireUnit 

# getFireWireUnit

Returns an IOFireWireUnit object.

``` source
virtual IOFireWireUnit * getFireWireUnit(
 void ); 
```

## Return Value

Returns a pointer to an IOFireWireUnit.

## Overview

An IOFireWireUnit is the provider of an IOFireWireSBP2Target. In order to use the base FireWire services you will need a reference to the unit. This method returns that reference.

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

getLUNumber

Returns the LUNs number.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

