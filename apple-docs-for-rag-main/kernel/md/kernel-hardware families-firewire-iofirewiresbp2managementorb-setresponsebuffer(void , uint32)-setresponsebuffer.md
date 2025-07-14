

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  setResponseBuffer(void \*, UInt32) 

# setResponseBuffer(void \*, UInt32)

Sets the response buffer for the management ORB.

``` source
virtual IOReturn setResponseBuffer(
 void *buf,
 UInt32len ); 
```

## Parameters 

`buf`  

backing store for buffer

`len`  

length of buffer.

## Return Value

Returns kIOReturnSuccess on a success.

## Overview

Sets the response buffer for the management ORB. kFWSBP2QueryLogins returns a response to its query and needs to write it somewhere. This routine allows you to specify the location.

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

setManageeCommand

Sets the command to be managed by the management ORB.

setResponseBuffer(IOMemoryDescriptor *)

Sets the response buffer for the management ORB.

