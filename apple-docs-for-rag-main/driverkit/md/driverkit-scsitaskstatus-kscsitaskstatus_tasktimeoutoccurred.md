

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_TaskTimeoutOccurred 

Enumeration Case

# kSCSITaskStatus_TaskTimeoutOccurred

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_TaskTimeoutOccurred
```

## Discussion

If a task is aborted by the SCSI Protocol Layer due to it exceeding the timeout value specified by the task, the task status shall be set to kSCSITaskStatus_TaskTimeoutOccurred.

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

kSCSITaskStatus_ProtocolTimeoutOccurred

kSCSITaskStatus_DeviceNotResponding

kSCSITaskStatus_DeviceNotPresent

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_No_Status

