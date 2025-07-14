

- DriverKit
-  SCSITaskStatus 

Enumeration

# SCSITaskStatus

Attributes for task status.

DriverKitiOSiPadOSmacOS

``` source
typedef enum SCSITaskStatus : unsigned int { ... } SCSITaskStatus;
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

## See Also

### Enumerations

IOLockAssertState

IORWLockAssertState

kC0DataMaxStringLen

kINQUIRY_ANSI_VERSION_Mask

kINQUIRY_ANSI_VERSION_NoClaimedConformance

kINQUIRY_ANSI_VERSION_SCSI_1_Compliant

kINQUIRY_ANSI_VERSION_SCSI_2_Compliant

kINQUIRY_ANSI_VERSION_SCSI_SPC_2_Compliant

kINQUIRY_ANSI_VERSION_SCSI_SPC_3_Compliant

kINQUIRY_ANSI_VERSION_SCSI_SPC_Compliant

kINQUIRY_Byte3_AERC_Bit

kINQUIRY_Byte3_AERC_Mask

kINQUIRY_Byte3_HISUP_Bit

kINQUIRY_Byte3_HISUP_Mask

kINQUIRY_Byte3_NORMACA_Bit

