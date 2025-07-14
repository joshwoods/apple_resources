

- Kernel
- Hardware Families
- FireWire
-  FWAsyncStreamCallback 

Type Alias

# FWAsyncStreamCallback

macOS 10.2+

``` source
typedef void (*FWAsyncStreamCallback)(void *refcon, IOReturn status, IOFireWireBus *bus, IOFWAsyncStreamCommand *fwCmd);
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

