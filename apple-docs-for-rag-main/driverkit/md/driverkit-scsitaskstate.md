

- DriverKit
-  SCSITaskState 

Enumeration

# SCSITaskState

Attributes for task state.

DriverKitiOSiPadOSmacOS

``` source
typedef enum SCSITaskState : unsigned int { ... } SCSITaskState;
```

## Overview

The Task State represents the current state of the task. The state is set to NEW_TASK when the task is created. The SCSI Protocol Layer will then adjust the state as the task is queued and during execution. The SCSI Application Layer can examine the state to monitor the progress of a task. The Task State can only be modified by the SCSI Protocol Layer. The SCSI Application Layer can only read the state.

## Topics

### Constants

kSCSITaskState_NEW_TASK

kSCSITaskState_ENABLED

kSCSITaskState_BLOCKED

kSCSITaskState_DORMANT

kSCSITaskState_ENDED

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

