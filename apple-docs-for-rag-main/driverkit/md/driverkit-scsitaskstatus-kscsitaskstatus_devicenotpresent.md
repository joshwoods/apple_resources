

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_DeviceNotPresent 

Enumeration Case

# kSCSITaskStatus_DeviceNotPresent

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_DeviceNotPresent
```

## Discussion

If the task is unable to be delivered because the device has been detached, the task status shall be set to kSCSITaskStatus_DeviceNotPresent. This will allow the SCSI Application Layer to halt the sending of tasks to the device and, if supported, perform any device failover or system cleanup.

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

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_No_Status

