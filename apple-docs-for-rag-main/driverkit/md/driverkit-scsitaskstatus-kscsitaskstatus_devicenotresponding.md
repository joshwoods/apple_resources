

- DriverKit
- SCSITaskStatus
-  kSCSITaskStatus_DeviceNotResponding 

Enumeration Case

# kSCSITaskStatus_DeviceNotResponding

DriverKitiOSiPadOSmacOS

``` source
kSCSITaskStatus_DeviceNotResponding
```

## Discussion

If a task is unable to be delivered due to a failure of the device not accepting the task or the device acknowledging the attempt to send it the device the task status shall be set to kSCSITaskStatus_DeviceNotResponding. This will allow the SCSI Application driver to perform the necessary steps to try to recover the device. This shall only be reported after the SCSI Protocol Layer driver has attempted all protocol specific attempts to recover the device.

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

kSCSITaskStatus_DeviceNotPresent

kSCSITaskStatus_DeliveryFailure

kSCSITaskStatus_No_Status

