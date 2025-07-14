

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Login
-  setUnsolicitedStatusNotifyProc 

# setUnsolicitedStatusNotifyProc

Sets the callback to be called on normal command status.

``` source
virtual void setUnsolicitedStatusNotifyProc(
 void *refCon,
 FWSBP2NotifyCallbackcallback ); 
```

## Parameters 

`refCon`  

refCon passed to callback.

`callback`  

address of callback method of type FWSBP2NotifyCallback.

## Overview

The supplied callback is called when unsolicited status is recieved. "notificationEvent" in the callback's params will indicate what happened. In this case it will be set to kFWSBP2UnsolicitedStatus. If "len" is non-zero then "message" contains the data written to the status block. Note: any buffers returned by callbacks are only valid for the duration of the login and should not have their contents modified.

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

submitFetchAgentReset

Resets the LUN's fetch agent.

submitLogin

Attempts to login to the LUN.

submitLogout

Attempts to logout of the LUN.

submitORB

Submits the given orb

