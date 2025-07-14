

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  attach 

# attach

Attaches an IOService client to a provider in the registry.

``` source
virtual bool attach(
 IOService *provider ); 
```

## Parameters 

`provider`  

The IOService object which will serve as this objects provider.

## Return Value

false if the provider is inactive or on a resource failure, otherwise true.

## Overview

See IOService for discussion.

## See Also

### Miscellaneous

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

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

