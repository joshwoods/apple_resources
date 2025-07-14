

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2Login 

Class

# IOFireWireSBP2Login

Supplies the login maintenance and Normal Command ORB execution portions of the API.

macOS 10.0+

``` source
class IOFireWireSBP2Login : OSObject
```

## Overview

Supplies APIs for login maintenance and command execution. Drivers can use this object to create IOFireWireSBP2ORB objects and execute them. Solicited and unsolicited status callback routines can be registered and the SBP2 services will notify the driver when the appropriate status arrives. This class also handles login maintenance. Supplies APIs for logging in and logging out and attempts to reconnect to the LUN after bus resets. The base FireWire services deliver bus reset notification via the IOKit message routine. The SBP2 services build on this behavior and deliver reconnectFailed and reconnectComplete through the message routine as well.

## Topics

### Miscellaneous

createORB

Creates a new IOFireWireSBP2ORB for this login.

enableUnsolicitedStatus

Enables unsolicited status.

getLoginFlags

Returns the currently set login flags.

getLoginID

Returns the current login ID.

getMaxCommandBlockSize

Returns the maximum command block size.

getMaxPayloadSize

Returns the currently set maximum payload size.

getReconnectTime

Returns the currently set reconnect time.

getRefCon

Returns the refCon set with setRefCon.

getStatusNotifyProc

Returns the callback to be called on normal command status.

getUnsolicitedStatusNotifyProc

Returns the callback to be called on unsolicited status.

release

Primary implementation of the release mechanism.

ringDoorbell

Rings the doorbell on the LUN.

setBusyTimeoutRegisterValue

Sets the value to be written to the BUSY_TIMEOUT register.

setFetchAgentResetCompletion

Sets the callback to be called when a fetch agent reset completes.

setFetchAgentWriteCompletion

Sets the callback to be called when the fetch agent write completes.

setLoginCompletion

Sets the callback to be called when a login attempt is complete.

setLoginFlags

Sets login configuration flags.

setLoginRetryCountAndDelayTime

Sets login retry behavior.

setLogoutCompletion

Sets the callback to be called when a logout attempt is complete.

setMaxPayloadSize

Sets the maximum data transfer length for a normal command ORB.

setPassword(IOMemoryDescriptor *)

Sets the login password.

setPassword(void *, UInt32)

Sets the login password.

setReconnectTime

Sets the desired reconnect duration.

setRefCon

Sets the login refCon.

setStatusNotifyProc

Sets the callback to be called on normal command status.

setUnsolicitedStatusNotifyProc

Sets the callback to be called on normal command status.

submitFetchAgentReset

Resets the LUN's fetch agent.

submitLogin

Attempts to login to the LUN.

submitLogout

Attempts to logout of the LUN.

submitORB

Submits the given orb

### Instance Methods

- abortLogin

- addORB

- allocateResources

- appendORB

- appendORBImmediate

- cancelORBTimer

- clearAllTasksInSet

- clearLoginGeneration

- completeLogin

- completeLogout

- createORB

- doReconnect

- doorbellComplete

- enableUnsolicitedStatus

- executeAddORB

- executeDoorbell

- executeFetchAgentReset

- executeLogin

- executeLogout

- executeORB

- executeRemoveORB

- executeSetBusyTimeout

- executeUnsolicitedStatusEnable

- fetchAgentResetComplete

- fetchAgentRetryTimer

- fetchAgentWriteComplete

- fetchAgentWriteComplete

- free

- getARDMMax

- getFireWireLUN

- getFireWireUnit

- getLoginFlags

- getLoginID

- getMaxCommandBlockSize

- getMaxPayloadSize

- getMetaClass

- getReconnectTime

- getRefCon

- getStatusNotifyProc

- getTarget

- getUnitInformation

- getUnsolicitedStatusNotifyProc

- initORBWithLogin

- initWithLUN

- initialExecuteLogin

- isConnected

- isFetchAgentWriteInProgress

- isORBAppended

- isORBTimerSet

- isPhysicalAccessEnabled

- loginRetryTimeout

- loginTimeout

- loginWriteComplete

- logoutTimeout

- logoutWriteComplete

- prepareORBForExecution

- processLoginWrite

- reconnectRetryTimeout

- reconnectStatusBlockWrite

- reconnectTimeout

- reconnectWriteComplete

- release

- removeLogin

- removeORB

- restartReconnect

- resumeNotify

- ringDoorbell

- sendReconnectNotification

- sendReconnectNotificationWithStatusBlock

- sendTimeoutNotification

- setAddressLoForLoginORBAndResponse

- setBusyTimeoutComplete

- setBusyTimeoutRegisterValue

- setFetchAgentResetCompletion

- setFetchAgentWriteCompletion

- setLoginCompletion

- setLoginFlags

- setLoginGeneration

- setLoginRetryCountAndDelayTime

- setLogoutCompletion

- setMaxPayloadSize

- setNextORBAddress

- setORBIsAppended

- setPassword

- setPassword

- setReconnectTime

- setRefCon

- setStatusNotifyProc

- setUnsolicitedStatusNotifyProc

- startFetchAgentRetryTimer

- startLoginRetryTimer

- startORBTimer

- startReconnectRetryTimer

- startReconnectTimer

- statusBlockWrite

- stopFetchAgentRetryTimer

- stopLoginRetryTimer

- stopReconnectRetryTimer

- submitFetchAgentReset

- submitLogin

- submitLogout

- submitORB

- suspendedNotify

- terminateNotify

- unsolicitedStatusEnableComplete

### Type Methods

+ doorbellCompleteStatic

+ fetchAgentResetCompleteStatic

+ fetchAgentRetryTimerStatic

+ fetchAgentWriteCompleteStatic

+ loginRetryTimeoutStatic

+ loginTimeoutStatic

+ loginWriteCompleteStatic

+ logoutTimeoutStatic

+ logoutWriteCompleteStatic

+ reconnectRetryTimeoutStatic

+ reconnectStatusBlockWriteStatic

+ reconnectTimeoutStatic

+ reconnectWriteCompleteStatic

+ setBusyTimeoutCompleteStatic

+ staticExecuteAddORB

+ staticExecuteDoorbell

+ staticExecuteFetchAgentReset

+ staticExecuteLogin

+ staticExecuteLogout

+ staticExecuteORB

+ staticExecuteRemoveORB

+ staticExecuteUnsolicitedStatusEnable

+ statusBlockWriteStatic

+ unsolicitedStatusEnableCompleteStatic

## Relationships

### Inherits From

- OSObject

## See Also

### Serial Bus Protocol 2

IOFireWireSBP2ManagementORB

Supplies non login related management ORBs. Management ORBs can be executed independent of a login, if necessary. Management ORBs are created using the IOFireWireSBP2LUN interface.

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

