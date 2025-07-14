

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2LUN
-  matchPropertyTable 

# matchPropertyTable

Implements SBP2 specific matching.

``` source
virtual bool matchPropertyTable(
 OSDictionary *table); 
```

## Parameters 

`table`  

The dictionary of properties to be matched against.

## Return Value

Returns false if the family considers the matching dictionary does not match in properties it understands, true otherwise.

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

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

