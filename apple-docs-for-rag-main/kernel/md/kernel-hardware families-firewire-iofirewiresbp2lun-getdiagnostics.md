

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  getDiagnostics 

# getDiagnostics

Debug-only method.

``` source
virtual OSObject * getDiagnostics(
 void ); 
```

## Return Value

Returns a pointer to the diagnostics object (if any).

## Overview

Returns a reference to the internal diagnostics object when the services are built in debug mode. Should be a no-op in release builds.

## See Also

### Miscellaneous

attach

Attaches an IOService client to a provider in the registry.

createLogin

Creates a new IOFireWireSBP2Login object.

createManagementORB

Creates a new IOFireWireSBP2ManagementORB object.

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

