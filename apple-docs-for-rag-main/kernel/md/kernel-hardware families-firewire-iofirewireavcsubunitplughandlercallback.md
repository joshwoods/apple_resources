

- Kernel
- Hardware Families
- FireWire
-  IOFireWireAVCSubunitPlugHandlerCallback 

Type Alias

# IOFireWireAVCSubunitPlugHandlerCallback

macOS 10.3+

``` source
typedef void (*IOFireWireAVCSubunitPlugHandlerCallback)(const AVCSubunitInfo *pSubunitInfo, IOFWAVCSubunitPlugMessages plugMessage, IOFWAVCPlugTypes plugType, UInt32 plugNum, UInt32 messageParams, UInt32 generation, UInt16 nodeID);
```

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

FWWriteCallback

Callback called when a write request packet is received for a 'virtual' firewire address.

