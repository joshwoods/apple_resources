

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  getResponseBuffer 

# getResponseBuffer

Returns the response buffer for the management ORB.

``` source
virtual void getResponseBuffer(
 void **buf,
 UInt32 *len ); 
```

## Parameters 

`desc`  

memory descriptor for buffer.

`buf`  

output parameter for backing store for buffer

`len`  

output parameter for length of buffer.

## Overview

Returns the response buffer set in setResponseBuffer above

## See Also

### Miscellaneous

getCommandFunction()

Returns the current function of the management ORB.

getCommandFunction()

Returns the current managee command of the management ORB.

getManageeCommand

Returns the current managee command of the management ORB.

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

