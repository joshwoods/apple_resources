

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2UserClient 

Class

# IOFireWireSBP2UserClient

macOS 10.0+

``` source
class IOFireWireSBP2UserClient : IOUserClient
```

## Topics

### Instance Methods

- LSIWorkaroundSetCommandBuffersAsRanges

- LSIWorkaroundSyncBuffersForInput

- LSIWorkaroundSyncBuffersForOutput

- checkArguments

- clientClose

- clientDied

- close

- createLogin

- createMgmtORB

- createORB

- enableUnsolicitedStatus

- externalMethod

- fetchAgentResetComplete

- fetchAgentWriteComplete

- flushAllManagementORBs

- free

- getLoginID

- getMaxCommandBlockSize

- getMetaClass

- getMgmtORBAsyncCallbackReference

- getSessionRef

- initWithTask

- loginCallback

- logoutCallback

- message

- mgmtORBCallback

- open

- openWithSessionRef

- releaseCommandBuffers

- releaseLogin

- releaseMgmtORB

- releaseORB

- ringDoorbell

- setBusyTimeoutRegisterValue

- setCommandBlock

- setCommandBuffersAsRanges

- setCommandFlags

- setCommandGeneration

- setCommandTimeout

- setFetchAgentWriteCompletion

- setLoginCallback

- setLoginFlags

- setLogoutCallback

- setMaxORBPayloadSize

- setMaxPayloadSize

- setMessageCallback

- setMgmtORBAsyncCallbackReference

- setMgmtORBCallback

- setMgmtORBCommandFunction

- setMgmtORBManageeLogin

- setMgmtORBManageeORB

- setMgmtORBResponseBuffer

- setORBRefCon

- setPassword

- setReconnectTime

- setStatusNotify

- setToDummy

- setUnsolicitedStatusNotify

- start

- statusNotify

- submitFetchAgentReset

- submitLogin

- submitLogout

- submitMgmtORB

- submitORB

- unsolicitedNotify

### Type Methods

+ staticFetchAgentResetComplete

+ staticFetchAgentWriteComplete

+ staticLoginCallback

+ staticLogoutCallback

+ staticMgmtORBCallback

+ staticStatusNotify

+ staticUnsolicitedNotify

## Relationships

### Inherits From

- IOUserClient

