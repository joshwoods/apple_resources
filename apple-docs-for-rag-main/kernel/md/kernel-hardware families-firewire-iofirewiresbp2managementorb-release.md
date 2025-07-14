

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ManagementORB
-  release 

# release

Primary implementation of the release mechanism.

``` source
virtual void release() const; 
```

## Parameters 

`when`  

When retainCount == when then call free().

## Overview

See OSObject.h for more information.

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

setCommandFunction

Sets the function of the management ORB.

setManageeCommand

Sets the command to be managed by the management ORB.

setResponseBuffer(IOMemoryDescriptor *)

Sets the response buffer for the management ORB.

setResponseBuffer(void *, UInt32)

Sets the response buffer for the management ORB.

