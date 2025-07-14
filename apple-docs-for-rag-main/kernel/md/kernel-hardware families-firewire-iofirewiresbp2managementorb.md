

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2ManagementORB 

Class

# IOFireWireSBP2ManagementORB

Supplies non login related management ORBs. Management ORBs can be executed independent of a login, if necessary. Management ORBs are created using the IOFireWireSBP2LUN interface.

macOS 10.0+

``` source
class IOFireWireSBP2ManagementORB : IOFWCommand
```

## Overview

## Topics

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

setResponseBuffer(void *, UInt32)

Sets the response buffer for the management ORB.

### Instance Methods

- allocateResources

- clearAllTasksInSet

- complete

- execute

- free

- getAsyncCallbackReference

- getCommandFunction

- getManageeCommand

- getMetaClass

- getResponseBuffer

- getUnitInformation

- handleTimeout

- initWithLUN

- release

- removeManagementORB

- setAsyncCallbackReference

- setCommandFunction

- setManageeCommand

- setORBToDummy

- setResponseBuffer

- setResponseBuffer

- statusBlockWrite

- suspendedNotify

- writeComplete

### Type Methods

+ handleTimeoutStatic

+ statusBlockWriteStatic

+ writeCompleteStatic

## Relationships

### Inherits From

- IOFWCommand

## See Also

### Serial Bus Protocol 2

IOFireWireSBP2Login

Supplies the login maintenance and Normal Command ORB execution portions of the API.

IOFireWireSBP2ORB

Represents an SBP2 normal command ORB. Supplies the APIs for configuring normal command ORBs. This includes setting the command block and writing the page tables for I/O. The ORBs are executed using the submitORB method in IOFireWireSBP2Login.

FWSBP2FetchAgentWriteCallback

FWSBP2LoginCallback

FWSBP2LoginCompleteParams

FWSBP2LoginCompleteParamsPtr

FWSBP2LoginResponse

FWSBP2LoginResponsePtr

FWSBP2LogoutCallback

FWSBP2LogoutCompleteParams

FWSBP2LogoutCompleteParamsPtr

FWSBP2ManagementCallback

FWSBP2NotifyCallback

FWSBP2NotifyParams

FWSBP2NotifyParamsPtr

FWSBP2ReconnectParams

FWSBP2ReconnectParamsPtr

FWSBP2StatusBlock

FWSBP2StatusCallback

