

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2Login
-  setBusyTimeoutRegisterValue 

# setBusyTimeoutRegisterValue

Sets the value to be written to the BUSY_TIMEOUT register.

``` source
virtual void setBusyTimeoutRegisterValue(
 UInt32timeout ); 
```

## Parameters 

`timeout`  

desired value of the BUSY_TIMEOUT register.

## Overview

1394-1995 defines a register known as the BUSY_TIMEOUT register. This register controls the busy retry behavior of your device. The initial value for this register is 0x00000000. Which means busied transactions will not be retried. Since most devices want their transactions retired on busy acks, the SBP2 service automatically updates the BUSY_TIMEOUT register with the value specified here whenever necessary. Most drivers should set this value to 0x0000000f.

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

