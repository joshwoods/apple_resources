

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  getCommandFunction() 

# getCommandFunction()

Returns the current managee command of the management ORB.

``` source
virtual OSObject* getManageeCommand(
 void ); 
```

## Return Value

Returns the current managee command of the management ORB.

## Overview

Returns the current managee command of the management ORB. This is the same value that was set with setManageeCommand.

## See Also

### Miscellaneous

getCommandFunction()

Returns the current function of the management ORB.

getManageeCommand

Returns the current managee command of the management ORB.

getResponseBuffer

Returns the response buffer for the management ORB.

release

Primary implementation of the release mechanism.

setCommandFunction

Sets the function of the management ORB.

setManageeCommand

Sets the command to be managed by the management ORB.

setResponseBuffer(IOMemoryDescriptor *)

Sets the response buffer for the management ORB.

setResponseBuffer(void *, UInt32)

Sets the response buffer for the management ORB.

