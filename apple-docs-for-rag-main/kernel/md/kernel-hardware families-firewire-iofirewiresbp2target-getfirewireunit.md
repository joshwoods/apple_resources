

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Target
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

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

