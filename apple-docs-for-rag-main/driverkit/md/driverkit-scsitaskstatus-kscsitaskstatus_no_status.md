

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_No_Status 

Enumeration Case

# kSCSITaskStatus_No_Status

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_No_Status
```

## Discussion

This status is not defined by the SCSI specifications, but is here to provide a status that can be returned in cases where there is not status available from the device or protocol, for example, when the service response is neither TASK_COMPLETED nor LINK_COMMAND_COMPLETE or when the service response is SERVICE_DELIVERY_OR_TARGET_FAILURE and the reason for failure could not be determined.

## See Also

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

