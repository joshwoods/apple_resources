

- Kernel
- Hardware Families
- SCSI
-  SCSIServiceResponse 

Enumeration

# SCSIServiceResponse

Attributes for task service response.

DriverKitKernelDriverKit 20.0+macOS 10.0+

**DriverKit**

``` source
typedef enum SCSIServiceResponse : unsigned int {
    ...
} SCSIServiceResponse;
```

**macOS**

``` source
typedef enum SCSIServiceResponse SCSIServiceResponse;
```

## Overview

The Service Response represents the execution status of a service request made to a Protocol Services Driver. The Service Response can only be modified by the SCSI Protocol Layer. The SCSI Application Layer can only read the state.

## Topics

### Constants

kSCSIServiceResponse_Request_In_Process

kSCSIServiceResponse_SERVICE_DELIVERY_OR_TARGET_FAILURE

kSCSIServiceResponse_TASK_COMPLETE

kSCSIServiceResponse_LINK_COMMAND_COMPLETE

kSCSIServiceResponse_FUNCTION_COMPLETE

kSCSIServiceResponse_FUNCTION_REJECTED

kSCSIServiceResponse_FUNCTION_COMPLETE

kSCSIServiceResponse_FUNCTION_REJECTED

kSCSIServiceResponse_LINK_COMMAND_COMPLETE

kSCSIServiceResponse_Request_In_Process

kSCSIServiceResponse_SERVICE_DELIVERY_OR_TARGET_FAILURE

kSCSIServiceResponse_TASK_COMPLETE

## See Also

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

