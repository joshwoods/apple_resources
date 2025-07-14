

- DriverKit
-  SCSITaskAttribute 

Enumeration

# SCSITaskAttribute

Attributes for task delivery.

DriverKitiOSiPadOSmacOS

``` source
typedef enum SCSITaskAttribute : unsigned int { ... } SCSITaskAttribute;
```

## Overview

The Task Attribute defines how this task should be managed when determing order for queueing and submission to the appropriate device server. The Task Attribute is set by the SCSI Application Layer and cannot be modified by the SCSI Protocol Layer.

## Topics

### Constants

kSCSITask_SIMPLE

kSCSITask_ORDERED

kSCSITask_HEAD_OF_QUEUE

kSCSITask_ACA

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

