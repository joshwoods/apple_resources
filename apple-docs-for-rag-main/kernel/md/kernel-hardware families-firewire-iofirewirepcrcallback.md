

- Kernel
- Hardware Families
- FireWire
-  IOFireWirePCRCallback 

Type Alias

# IOFireWirePCRCallback

Callback called after a successful lock transaction to a plug.

macOS 10.2+

``` source
typedef void (*IOFireWirePCRCallback)(void *refcon, UInt16 nodeID, UInt32 plug, UInt32 oldVal, UInt32 newVal);
```

## Parameters 

`refcon`  

refcon supplied to the IOFireWireFCPSpace when a client is registered

`nodeID`  

is the node originating the request

`plugNo`  

is the plug number

`oldVal`  

is the value the plug used to contain

`newVal`  

is the quad written into the plug

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

