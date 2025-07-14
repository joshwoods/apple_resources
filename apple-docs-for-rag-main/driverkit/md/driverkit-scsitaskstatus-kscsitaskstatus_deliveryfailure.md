

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_DeliveryFailure 

Enumeration Case

# kSCSITaskStatus_DeliveryFailure

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_DeliveryFailure
```

## Discussion

If the task is unable to be delivered to the device due to a failure in the SCSI Protocol Layer, such as a bus reset or communications error, but the device is is known to be functioning properly, the task status shall be set to kSCSITaskStatus_DeliveryFailure. This can also be reported if the task could not be delivered due to a protocol error that has since been corrected.

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

kSCSITaskStatus_No_Status

