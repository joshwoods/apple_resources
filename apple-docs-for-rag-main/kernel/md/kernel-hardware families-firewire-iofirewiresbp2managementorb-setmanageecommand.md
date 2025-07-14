

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  setManageeCommand 

# setManageeCommand

Sets the command to be managed by the management ORB.

``` source
virtual void setManageeCommand(
 OSObject *command ); 
```

## Parameters 

`command`  

a reference to an IOFireWireSBP2Login or an IOFireWireSBP2ORB.

## Overview

All management functions except kFWSBP2QueryLogins require a reference to an ORB of some sort. kFWSBP2AbortTaskSet, kFWSBP2LogicalUnitReset, and kFWSBP2TargetReset require a reference to the login ORB. kFWSBP2AbortTask requires a reference to the ORB to be aborted. This method allows you to set the ORB to be managed.

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

setCommandFunction

Sets the function of the management ORB.

setResponseBuffer(IOMemoryDescriptor *)

Sets the response buffer for the management ORB.

setResponseBuffer(void *, UInt32)

Sets the response buffer for the management ORB.

