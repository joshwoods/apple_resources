

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_ProtocolTimeoutOccurred 

Enumeration Case

# kSCSITaskStatus_ProtocolTimeoutOccurred

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_ProtocolTimeoutOccurred
```

## Discussion

If a task is aborted by the SCSI Protocol Layer due to it exceeding a timeout value specified by the support for the protocol or a related specification, the task status shall be set to kSCSITaskStatus_ProtocolTimeoutOccurred.

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

kSCSITaskStatus_DeviceNotResponding

kSCSITaskStatus_DeviceNotPresent

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_No_Status

