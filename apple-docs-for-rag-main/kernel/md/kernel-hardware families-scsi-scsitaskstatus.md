

- Kernel
- Hardware Families
- SCSI
-  SCSITaskStatus 

Enumeration

# SCSITaskStatus

Attributes for task status.

DriverKitKernelDriverKit 20.0+macOS 10.0+

**DriverKit**

``` source
typedef enum SCSITaskStatus : unsigned int {
    ...
} SCSITaskStatus;
```

**macOS**

``` source
typedef enum SCSITaskStatus SCSITaskStatus;
```

## Overview

The Task Status represents the completion status of the task which provides the SCSI Application Layer with additional information about how to procede in handling a completed task.

The SCSI Architecture Model specification only defines task status values for when a task completes with a service response of either TASK_COMPLETED or LINK_COMMAND_COMPLETE.

Since additional information will aid in error recovery when a task fails to be completed by a device due to a service response of kSCSIServiceResponse_SERVICE_DELIVERY_OR_TARGET_FAILURE, additional values have been defined that can be returned by the SCSI Protocol Layer to inform the SCSI Application Layer of the cause of the delivery failure.

The Task Status can only be modified by the SCSI Protocol Layer. The SCSI Application Layer can only read the status

## Topics

### Constants

kSCSITaskStatus_GOOD

kSCSITaskStatus_CHECK_CONDITION

kSCSITaskStatus_CONDITION_MET

kSCSITaskStatus_BUSY

kSCSITaskStatus_INTERMEDIATE

kSCSITaskStatus_INTERMEDIATE_CONDITION_MET

kSCSITaskStatus_RESERVATION_CONFLICT

kSCSITaskStatus_TASK_SET_FULL

kSCSITaskStatus_ACA_ACTIVE

kSCSITaskStatus_TaskTimeoutOccurred

kSCSITaskStatus_ProtocolTimeoutOccurred

kSCSITaskStatus_DeviceNotResponding

kSCSITaskStatus_DeviceNotPresent

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_No_Status

kSCSITaskStatus_ACA_ACTIVE

kSCSITaskStatus_BUSY

kSCSITaskStatus_CHECK_CONDITION

kSCSITaskStatus_CONDITION_MET

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_DeviceNotPresent

kSCSITaskStatus_DeviceNotResponding

kSCSITaskStatus_GOOD

kSCSITaskStatus_INTERMEDIATE

kSCSITaskStatus_INTERMEDIATE_CONDITION_MET

kSCSITaskStatus_No_Status

kSCSITaskStatus_ProtocolTimeoutOccurred

kSCSITaskStatus_RESERVATION_CONFLICT

kSCSITaskStatus_TASK_SET_FULL

kSCSITaskStatus_TaskTimeoutOccurred

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

