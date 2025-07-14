

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  setCommandFunction 

# setCommandFunction

Sets the function of the management ORB.

``` source
virtual IOReturn setCommandFunction(
 UInt32function ); 
```

## Parameters 

`function`  

a value indicating the desired management function.

## Return Value

Returns kIOReturnSuccess if function was a legal function.

## Overview

Sets the the function of the management ORB. Legal values are kFWSBP2QueryLogins, kFWSBP2AbortTask, kFWSBP2AbortTaskSet, kFWSBP2LogicalUnitReset, and kFWSBP2TargetReset.

## See Also

### Miscellaneous

getCommandFunction()

Returns the current function of the management ORB.

getCommandFunction()

Returns the current managee command of the management ORB.

getManageeCommand

Returns the current managee command of the management ORB.

getResponseBuffer

Returns the response buffer for the management ORB.

release

Primary implementation of the release mechanism.

setManageeCommand

Sets the command to be managed by the management ORB.

setResponseBuffer(IOMemoryDescriptor *)

Sets the response buffer for the management ORB.

setResponseBuffer(void *, UInt32)

Sets the response buffer for the management ORB.

