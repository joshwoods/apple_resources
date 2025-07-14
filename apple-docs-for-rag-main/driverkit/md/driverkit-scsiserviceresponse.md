

- DriverKit
-  SCSIServiceResponse 

Enumeration

# SCSIServiceResponse

Attributes for task service response.

DriverKitiOSiPadOSmacOS

``` source
typedef enum SCSIServiceResponse : unsigned int { ... } SCSIServiceResponse;
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

