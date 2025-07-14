

- Kernel
- Hardware Families
- SCSI
-  IOSCSIReducedBlockCommandsDevice 

Class

# IOSCSIReducedBlockCommandsDevice

macOS 10.6+

``` source
class IOSCSIReducedBlockCommandsDevice : IOSCSIPrimaryCommandsDevice
```

## Topics

### Instance Methods

- AsyncReadWrite

- AsyncReadWriteCompletion

- CheckMediaPresence

- CheckWriteProtection

- ClearNotReadyStatus

- CreateStorageServiceNub

- DetermineDeviceCharacteristics

- DisablePolling

- EjectTheMedia

- EnablePolling

- FORMAT_UNIT

- FormatMedia

- GetFormatCapacities

- GetInitialPowerState

- GetNumberOfPowerStateTransitions

- HandleCheckPowerState

- HandlePowerChange

- INQUIRY

- InitializeDeviceSupport

- InitializePowerManagement

- IssueRead

- IssueRead

- IssueWrite

- IssueWrite

- LockUnlockMedia

- MODE_SELECT_6

- MODE_SENSE_6

- PERSISTENT_RESERVE_IN

- PERSISTENT_RESERVE_OUT

- PREVENT_ALLOW_MEDIUM_REMOVAL

- PollForMedia

- PowerDownHandler

- READ_10

- READ_CAPACITY

- RELEASE_6

- REQUEST_SENSE

- RESERVE_6

- ReportBlockSize

- ReportEjectability

- ReportLockability

- ReportMaxReadTransfer

- ReportMaxValidBlock

- ReportMaxWriteTransfer

- ReportMediaState

- ReportPollRequirements

- ReportRemovability

- ReportWriteProtection

- ResetMediaCharacteristics

- ResumeDeviceSupport

- START_STOP_UNIT

- SYNCHRONIZE_CACHE

- SetMediaCharacteristics

- SetMediaIcon

- StartDeviceSupport

- StopDeviceSupport

- SuspendDeviceSupport

- SyncReadWrite

- SynchronizeCache

- TEST_UNIT_READY

- TerminateDeviceSupport

- TicklePowerManager

- VERIFY

- WRITE_10

- WRITE_BUFFER

- free

- getMetaClass

### Type Methods

+ AsyncReadWriteComplete

+ sPollForMedia

## Relationships

### Inherits From

- IOSCSIPrimaryCommandsDevice

## See Also

### Block Devices

IOSCSIPeripheralDeviceType00

IOSCSIPeripheralDeviceType07

IOSCSIPeripheralDeviceType0E

IOSCSIBlockCommandsDevice

