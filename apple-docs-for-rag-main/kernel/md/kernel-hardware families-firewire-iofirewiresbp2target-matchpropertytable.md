

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
-  matchPropertyTable 

# matchPropertyTable

Implements SBP2 specific matching.

``` source
virtual bool matchPropertyTable(
 OSDictionary *table ); 
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

getFireWireUnit

Returns an IOFireWireUnit object.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

