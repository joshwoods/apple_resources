

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  createManagementORB 

# createManagementORB

Creates a new IOFireWireSBP2ManagementORB object.

``` source
virtual IOFireWireSBP2ManagementORB * createManagementORB(
 void *refCon,
 FWSBP2ManagementCallbackcompletion ); 
```

## Parameters 

`refCon`  

The refcon passed to the completion routine.

`completion`  

The completion routine. Called when the ORB finishes execution.

## Return Value

Returns a pointer to a new IOFireWireSBP2Login.

## Overview

Creates a new IOFireWireSBP2ManagementORB object. Management objects let you execute commands like QueryLogins, LogicalUnitReset, and AbortTask. These commands are configured after they are created here. When they are done executing (after a call to submit) the supplied completion routine will be called with the supplied refcon. Usually this refCon is the "this" pointer of completion method's object.

## See Also

### Miscellaneous

attach

Attaches an IOService client to a provider in the registry.

createLogin

Creates a new IOFireWireSBP2Login object.

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

