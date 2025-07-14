

- Kernel
- Hardware Families
- FireWire
-  IOFWCmdQ 

# IOFWCmdQ

Structure for head of a queue of IOFWCommands

macOS 10.6+

``` source
struct IOFWCmdQ {
    ...
};
```

## Topics

### Fields

fHead

Points to the head of the queue, or NULL if queue is empty

fTail

Points to the tail of the queue, or NULL if queue is empty

headChanged

called when head command is changed, or the command itself changes state.

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

FWWriteCallback

Callback called when a write request packet is received for a 'virtual' firewire address.

