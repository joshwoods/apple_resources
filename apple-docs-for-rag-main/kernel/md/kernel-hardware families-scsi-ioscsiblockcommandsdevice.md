

- Kernel
- Hardware Families
- SCSI
-  IOSCSIBlockCommandsDevice 

Class

# IOSCSIBlockCommandsDevice

macOS 10.6+

``` source
class IOSCSIBlockCommandsDevice : IOSCSIPrimaryCommandsDevice
```

## Topics

### Instance Methods

- AsyncReadWrite

- AsyncReadWrite

- AsyncReadWriteCompletion

- CheckMediumCapacityData

- ClearNotReadyStatus

- CreateStorageServiceNub

- DetermineDeviceCharacteristics

- DetermineMediaPresence

- DetermineMediumCapacity

- DetermineMediumGeometry

- DetermineMediumWriteProtectState

- DisablePolling

- EjectTheMedium

- EnablePolling

- FormatMedium

- GET_LBA_STATUS

- GetDeviceUnmapCharacteristics

- GetFormatCapacities

- GetInitialPowerState

- GetMediumRotationRate

- GetNumberOfPowerStateTransitions

- GetProvisionStatus

- GetWriteCacheState

- GetWriteCacheState

- HandleCheckPowerState

- HandlePowerChange

- InitializeDeviceSupport

- InitializePowerManagement

- IsUnmapAllowed

- IsUseWriteSame

- IssueRead

- IssueRead

- IssueUnmap

- IssueWrite

- IssueWrite

- LockUnlockMedium

- LogicalBlockProvisioningUnmapSupport

- PollForMediaRemoval

- PollForNewMedia

- PowerDownHandler

- PreventMediumRemoval

- ProcessPoll

- READ_10

- READ_10

- READ_12

- READ_12

- READ_16

- READ_CAPACITY

- READ_CAPACITY_16

- REPORT_PROVISIONING_INITIALIZATION_PATTERN

- ReportDeviceMaxBlocksReadTransfer

- ReportDeviceMaxBlocksWriteTransfer

- ReportDeviceMediaRemovability

- ReportMediumBlockSize

- ReportMediumTotalBlockCount

- ReportMediumWriteProtection

- ReportProvisioningInitializationPattern

- ResetMediumCharacteristics

- ResumeDeviceSupport

- START_STOP_UNIT

- SYNCHRONIZE_CACHE

- SYNCHRONIZE_CACHE

- SYNCRONIZE_CACHE_16

- SetMediumCharacteristics

- SetMediumCharacteristics

- SetMediumIcon

- SetWriteCacheState

- StartDeviceSupport

- StopDeviceSupport

- SuspendDeviceSupport

- SyncReadWrite

- SynchronizeCache

- TerminateDeviceSupport

- TicklePowerManager

- UNMAP

- Unmap

- UnmapTruncateAndAccumulate

- UnmapTryExtentCoalesce

- UpdateLBAProvisionStatus

- VerifyMediumPresence

- WRITE_10

- WRITE_10

- WRITE_12

- WRITE_12

- WRITE_16

- WRITE_SAME_10

- WRITE_SAME_16

- WriteSame

- WriteSameUnmap

- free

- getMetaClass

- message

- systemWillShutdown

### Type Methods

+ AbortPMTransition

+ AsyncReadWriteComplete

+ sProcessPoll

## Relationships

### Inherits From

- IOSCSIPrimaryCommandsDevice

## See Also

### Block Devices

IOSCSIPeripheralDeviceType00

IOSCSIPeripheralDeviceType07

IOSCSIPeripheralDeviceType0E

IOSCSIReducedBlockCommandsDevice

