

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2LUN 

Class

# IOFireWireSBP2LUN

Provider for most drivers.

macOS 10.0+

``` source
class IOFireWireSBP2LUN : IOService
```

## Overview

IOFireWireSBP2LUN objects are created by IOFireWireSBP2Target objects. Each target may have zero or more IOFireWireSBP2LUN children. The LUN object serves as the matching nub for most drivers and therefore will be the provider for most drivers. It supplies the methods that control the operation of the LUN as a whole. Methods that control the behavior and execution of an SBP2 login session are supplied in a separate IOFireWireSBP2Login object. The LUN can be used to create one of these login objects. The LUN can also create IOFireWireSBP2ManagementORBs for configuring and appending non-login related management functions. Login related management functions (ie. Login, Logout, Reconnect) are supplied by the IOFireWireSBP2Login. Finally the LUN can supply a reference to the IOFireWireUnit. This can be useful if a driver wishes to access the standard FireWire APIs.

## Topics

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

matchPropertyTable

Implements SBP2 specific matching.

### Instance Methods

- attach

- clearAllTasksInSet

- createLogin

- createLoginAction

- createManagementORB

- createManagementORBAction

- executeFlushAllMgmtORBs

- finalize

- flushAllManagementORBs

- free

- getDiagnostics

- getFireWireUnit

- getLUNumber

- getMetaClass

- getTarget

- handleClose

- handleOpen

- initLoginWithLUN

- initMgmtORBWithLUN

- matchPropertyTable

- message

- removeLogin

- removeLoginAction

- removeManagementORB

- removeManagementORBAction

- resumeNotify

- suspendedNotify

- terminateNotify

### Type Methods

+ staticCreateLogin

+ staticCreateManagementORBAction

+ staticExecuteFlushAllMgmtORBs

+ staticRemoveLoginAction

+ staticRemoveManagementORBAction

## Relationships

### Inherits From

- IOService

## See Also

### Nubs

IOFireWireLocalNode

IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireAVCNub

nub for AVC devices

IOFireWireUnit

IOFireWireNub

