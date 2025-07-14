

- Kernel
- Hardware Families
-  SCSI 

API Collection

# SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

## Topics

### Block Devices

IOSCSIPeripheralDeviceType00

IOSCSIPeripheralDeviceType07

IOSCSIPeripheralDeviceType0E

IOSCSIBlockCommandsDevice

IOSCSIReducedBlockCommandsDevice

### Multimedia Devices

IOSCSILogicalUnitNub

IOSCSIParallelInterfaceController

Class that represents a SCSI Host Bus Adapter.

Deprecated

IOSCSIPeripheralDeviceType05

IOSCSIMultimediaCommandsDevice

### Base Types

IOReducedBlockServices

IOSCSIPeripheralDeviceNub

IOSCSIPrimaryCommandsDevice

IOSCSIProtocolServices

This class defines the public SCSI Protocol Services Layer API for any class that implements SCSI protocol services. A protocol services layer driver is responsible for taking incoming SCSITaskIdentifier objects and translating them to the native command type for the native protocol interface (e.g. SBP-2 ORB on FireWire).

IOSCSIProtocolInterface

This class defines the public SCSI Protocol Layer API for any class that provides Protocol services or needs to provide the Protocol Service API for passing service requests to a Protocol Service driver.

### Additional Types

SCSICmd_INQUIRY_PAGECx_Header

SCSICmd_INQUIRY_Page00_Header_SPC_16

SCSICmd_INQUIRY_Page80_Header_SPC_16

SCSICmd_INQUIRY_PageB0_Data

SCSICmd_INQUIRY_PageB2_Data

SCSICmd_INQUIRY_PageB2_Provisioning_Group_Descriptor

SCSICmd_INQUIRY_PageC0_Data

SCSICmd_INQUIRY_PageC1_Data

SCSICmd_INQUIRY_StandardDataPtr

SCSICmd_REPORT_LUNS_Header

SCSICmd_REPORT_LUNS_LUN_ENTRY

SCSICommandDescriptorBlock

SCSIDeviceIdentifier

64-bit number to represent a SCSI Device.

SCSIInitiatorIdentifier

64-bit number to represent a SCSI Initiator Device.

SCSILogicalUnitBytes

SCSILogicalUnitNumber

SCSIParallelMessages

SCSIParallelTaskIdentifier

SCSIPortStatus

32-bit number to represent a SCSIPortStatus.

SCSIProtocolFeature

SCSIProtocolPowerState

SCSIServiceResponse

Attributes for task service response.

SCSITaggedTaskIdentifier

64-bit number to represent a unique task identifier.

SCSITargetIdentifier

64-bit number to represent a SCSI Target Device.

SCSITaskAttribute

Attributes for task delivery.

SCSITaskState

Attributes for task state.

SCSITaskStatus

Attributes for task status.

SCSI_Sense_Data

SCSICmdField10Bit

SCSICmdField11Bit

SCSICmdField12Bit

SCSICmdField13Bit

SCSICmdField14Bit

SCSICmdField15Bit

SCSICmdField17Bit

SCSICmdField18Bit

SCSICmdField19Bit

SCSICmdField1Bit

SCSICmdField1Byte

SCSICmdField20Bit

SCSICmdField21Bit

SCSICmdField22Bit

SCSICmdField23Bit

SCSICmdField25Bit

SCSICmdField26Bit

SCSICmdField27Bit

SCSICmdField28Bit

SCSICmdField29Bit

SCSICmdField2Bit

SCSICmdField2Byte

SCSICmdField30Bit

SCSICmdField31Bit

SCSICmdField33Bit

SCSICmdField34Bit

SCSICmdField35Bit

SCSICmdField36Bit

SCSICmdField37Bit

SCSICmdField38Bit

SCSICmdField39Bit

SCSICmdField3Bit

SCSICmdField3Byte

SCSICmdField41Bit

SCSICmdField42Bit

SCSICmdField43Bit

SCSICmdField44Bit

SCSICmdField45Bit

SCSICmdField46Bit

SCSICmdField47Bit

SCSICmdField49Bit

SCSICmdField4Bit

SCSICmdField4Byte

SCSICmdField50Bit

SCSICmdField51Bit

SCSICmdField52Bit

SCSICmdField53Bit

SCSICmdField54Bit

SCSICmdField55Bit

SCSICmdField57Bit

SCSICmdField58Bit

SCSICmdField59Bit

SCSICmdField5Bit

SCSICmdField5Byte

SCSICmdField60Bit

SCSICmdField61Bit

SCSICmdField62Bit

SCSICmdField63Bit

SCSICmdField6Bit

SCSICmdField6Byte

SCSICmdField7Bit

SCSICmdField7Byte

SCSICmdField8Byte

SCSICmdField9Bit

## See Also

### Interfaces

Audio

Implement a driver that interacts with audio hardware.

Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

