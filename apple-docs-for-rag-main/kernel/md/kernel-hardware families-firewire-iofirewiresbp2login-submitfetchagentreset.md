

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Login
-  submitFetchAgentReset 

# submitFetchAgentReset

Resets the LUN's fetch agent.

``` source
virtual IOReturn submitFetchAgentReset(
 void ); 
```

## Return Value

Returns kIOReturnSuccess if the reset started successfully.

## Overview

The fetch agent state machine on the device can be reset by a write to a specific register. This reset can be intiated by a call to this method. Notification of the completion of this write can be had by registering a callback with the setFetchAgentResetCompletion method.

## See Also

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

submitLogin

Attempts to login to the LUN.

submitLogout

Attempts to logout of the LUN.

submitORB

Submits the given orb

