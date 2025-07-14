

- Kernel
- Hardware Families
-  FireWire 

API Collection

# FireWire

Implement a driver that supports FireWire devices.

## Topics

### Interfaces

IOFireWireSerialBusProtocolTransport

SCSI Protocol Driver Family for FireWire SBP2 Devices.

IOFireWireSBP2Target

Serves as bridge between IOFireWireUnit and IOFireWireLUN.

IOFireWireController

IOFireWireBus

IOFireWireBus is a public class the provides access to general FireWire functionality...

### Nubs

IOFireWireLocalNode

IOFireWireSBP2LUN

Provider for most drivers.

IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireAVCNub

nub for AVC devices

IOFireWireUnit

IOFireWireNub

### Devices

IOFireWireDevice

Represents a FireWire device.

### Auxilliary Units

IOFireWireControllerAux

IOFireWireLocalNodeAux

IOFireWireBusAux

IOFireWireDeviceAux

IOFireWireUnitAux

IOFireWireNubAux

### User-Space Access

IOFireWireSBP2UserClient

### AVC Support

IOFireWireAVCAsynchronousCommand

IOFireWireAVCTargetSpace

object to centralize the AVC Target mode support

IOFireWireAVCCommand

AVCCommandHandlerInfo

AVCConnectionRecord

AVCSubunitInfo

AVCConnectTargetPlugsInParams

AVCConnectTargetPlugsOutParams

AVCGetTargetPlugConnectionInParams

AVCGetTargetPlugConnectionOutParams

AVCSubunitPlugRecord

AVCUnitPlugRecord

AVCUnitPlugs

### DCL Support

IODCLProgram

IODCLTranslateListen

IODCLTranslateTalk

IODCLTranslator

IOFWReceiveDCL

IOFWSendDCL

IOFWSkipCycleDCL

IOFWDCL

DCLCallCommandProc

DCLCallCommandProcPtr

DCLCallProc

DCLCallProcDataType

DCLCallProcPtr

DCLCommand

DCLCommandPtr

DCLCompilerDataType

DCLJump

DCLJumpPtr

DCLLabel

DCLLabelPtr

DCLNuDCLLeader

DCLPtrTimeStamp

DCLPtrTimeStampPtr

DCLSetTagSyncBits

DCLSetTagSyncBitsPtr

DCLTimeStamp

DCLTimeStampPtr

DCLTransferBuffer

DCLTransferBufferPtr

DCLTransferPacket

DCLTransferPacketPtr

DCLUpdateDCLList

DCLUpdateDCLListPtr

### Serial Bus Protocol 2

IOFireWireSBP2Login

Supplies the login maintenance and Normal Command ORB execution portions of the API.

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

### Address Spaces

IOFWAddressSpaceAux

IOFWPhysicalAddressSpaceAux

IOFWPseudoAddressSpaceAux

IOFWSimpleContiguousPhysicalAddressSpace

IOFireWirePCRSpace

object to multiplex users of the PCR plug registers

IOFWPseudoAddressSpace

IOFWSimplePhysicalAddressSpace

IOFWPhysicalAddressSpace

IOFWAddressSpace

### Commands

IOFWCompareAndSwapCommand

IOFWAsyncCommand

Send an async request to a device

IOFWAsyncPHYCommand

Send an async PHY packet

IOFWAsyncStreamCommand

Send an async stream packet

IOFWBusCommand

Bus control commands

IOFWCommand

Base class for FireWire commands

IOFWDelayCommand

Command to execute some code after a specified delay (in microseconds) All it does is timeout after the specified delay, hence calling the completion callback.

IOFWReadCommand

IOFWReadQuadCommand

An easier to use version of IOFWReadCommand for use when the data to be transferred is an integer number of quads. Note that block read requests will be used for transfers greater than one quad unless setMaxPacket(4) is called.

IOFWWriteCommand

IOFWWriteQuadCommand

An easier to use version of IOFWWriteCommand for use when the data to be transferred is small and an integer number of quads. Note that block read requests will be used for transfers greater than one quad unless setMaxPacket(4) is called. kMaxWriteQuads is the largest legal number of quads that this object can be asked to transfer (the data is copied into an internal buffer in init() and reinit()).

### Utilities

SubtractFWCycleTimeFromFWCycleTime

AddFWCycleTimeToFWCycleTime

IOFWGetAbsoluteTime

FWComputeCRC16

FWUpdateCRC16

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

FWWriteCallback

Callback called when a write request packet is received for a 'virtual' firewire address.

### Global IDs

gFireWireModel_ID

gFireWireNodeID

gFireWireProduct_Name

gFireWireROM

gFireWireSelfIDs

gFireWireSpeed

gFireWireTDM

gFireWireUnit_SW_Version

gFireWireUnit_Spec_ID

gFireWireVendor_ID

gFireWireVendor_Name

gFireWire_GUID

### FireWire Types

UCInfo

IOLocalConfigDirectory

IOConfigDirectory

IOFireWireDuplicateGUIDList

IOFireWireIRMAllocation

IOFireWireMultiIsochReceiveListener

IOFWPHYPacketListener

IOFireWireMultiIsochReceivePacket

IOFireWirePowerManager

IOFWIsochChannel

IOFWIsochPort

IOFWLocalIsochPort

IOFWSyncer

IOFWUserObjectExporter

## See Also

### Hardware Interconnects

ATA

Implement a driver that supports Advanced Technology Attachment (ATA) devices.

Bluetooth

Implement a driver that supports Bluetooth devices.

PCI

Implement a driver that supports Thunderbolt devices or PCI cards.

USB

Implement a driver that supports Universal Serial Bus (USB) devices.

