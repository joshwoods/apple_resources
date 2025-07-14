

- Kernel
- Hardware Families
- FireWire
-  FWWriteCallback 

Type Alias

# FWWriteCallback

Callback called when a write request packet is received for a 'virtual' firewire address.

macOS 10.0+

``` source
typedef UInt32 (*FWWriteCallback)(void *refcon, UInt16 nodeID, IOFWSpeed & speed, FWAddress addr, UInt32 len, const void *buf, IOFWRequestRefCon requestRefcon);
```

## Parameters 

`device`  

is the node originating the request

`speed`  

is the FireWire speed of the request, update it if you need to control the speed of the reply, otherwise the response will be the same speed.

`addr`  

is the address the device is requesting to write to

`len`  

is the number of bytes to write

`buf`  

contains the packet data

`requestRefcon`  

refcon Can be queried for extra info about the request, using IOFireWireController::isLockRequest(), isQuadRequest()

## Return Value

return: kFWResponseComplete = 0, OK kFWResponseConflictError = 4, Resource conflict, may retry kFWResponseDataError = 5, Data not available kFWResponseTypeError = 6, Operation not supported kFWResponseAddressError = 7 Address not valid in target device

## See Also

### Types

IOFWDuplicateGUIDRec

IOFWARxReqIntCompleteHandler

IOFWAVCAsyncCommandState

IOFWAVCPlugTypes

IOFWAVCProtocolUserClientAsyncCommandCodes

IOFWAVCProtocolUserClientCommandCodes

IOFWAVCSubunitPlugMessages

IOFWAVCUserClientAsyncCommandCodes

IOFWAVCUserClientCommandCodes

IOFWCmdQ

Structure for head of a queue of IOFWCommands

IOFWDCLNotificationType

IOFWIsochPortOptions

IOFWIsochResourceFlags

IOFWNodeScan

IOFWPhysicalAccessMode

IOFWReadFlags

IOFWRequestRefCon

IOFWSBP2UserClientCommandCodes

IOFWSecurityMode

IOFWSpeed

IOFWWriteFlags

IOFireWireAVCAsynchronousCommandCallback

IOFireWireAVCSubunitPlugHandlerCallback

IOFireWireAVCTargetCommandHandlerCallback

IOFireWirePCRCallback

Callback called after a successful lock transaction to a plug.

IOFireWireSessionRef

IOAVCCommandResponse

IOAVCFrameFields

IOAVCOpcodes

IOAVCUnitTypes

FWAddress

FWAddressPtr

FWAsyncPHYCallback

FWAsyncStreamCallback

FWAsyncStreamReceiveCallback

FWBusCallback

FWClientCommandID

FWDeviceCallback

FWIsochChannelForceStopNotificationProc

FWIsochChannelForceStopNotificationProcPtr

FWMultiIsochReceiveListenerCallback

FWPHYPacketCallback

FWReadCallback

Callback called when a read request packet is received for a 'virtual' firewire address.

FWSegment

