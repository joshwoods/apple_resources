

- Kernel
- Hardware Families
- SCSI
-  IOSCSIMultimediaCommandsDevice 

Class

# IOSCSIMultimediaCommandsDevice

macOS 10.6+

``` source
class IOSCSIMultimediaCommandsDevice : IOSCSIPrimaryCommandsDevice
```

## Topics

### Instance Methods

- AsyncReadCD

- AsyncReadWrite

- AsyncReadWriteCompletion

- CheckForBDMediaType

- CheckForCDMediaType

- CheckForDVDMediaType

- CheckForLowPowerPollingSupport

- CheckMediaPresence

- CheckWriteProtection

- ClearNotReadyStatus

- ConvertBCDToHex

- ConvertMSFToLBA

- CreateStorageServiceNub

- DetermineDeviceCharacteristics

- DetermineDeviceFeatures

- DetermineIfMediaIsRemovable

- DetermineMediaType

- DisablePolling

- EjectTheMedia

- EnablePolling

- FormatMedia

- GET_CONFIGURATION

- GET_EVENT_STATUS_NOTIFICATION

- GET_PERFORMANCE

- GetBlockSize

- GetCurrentPowerStateOfDrive

- GetDeviceConfiguration

- GetDeviceConfigurationSize

- GetFormatCapacities

- GetInitialPowerState

- GetMechanicalCapabilities

- GetMechanicalCapabilitiesSize

- GetMediaAccessSpeed

- GetMediaType

- GetNumberOfPowerStateTransitions

- GetTrayState

- HandleCheckPowerState

- HandlePowerChange

- HandleSetUserClientExclusivityState

- InitializeDeviceSupport

- InitializePowerManagement

- IssueRead

- IssueRead

- IssueWrite

- IssueWrite

- LOAD_UNLOAD_MEDIUM

- LockUnlockMedia

- MECHANISM_STATUS

- ParseFeatureList

- ParseMechanicalCapabilities

- PollForMedia

- PowerDownHandler

- READ_10

- READ_CAPACITY

- READ_CD

- READ_CD_MSF

- READ_DISC_INFORMATION

- READ_DISC_STRUCTURE

- READ_DVD_STRUCTURE

- READ_FORMAT_CAPACITIES

- READ_SUB_CHANNEL

- READ_TOC_PMA_ATIP

- READ_TRACK_INFORMATION

- REPORT_KEY_V2Deprecated

- REPORT_KEY_V3

- RESERVE_TRACK_V2

- ReadDVDStructure

- ReadDiscInfo

- ReadDiscStructure

- ReadISRC

- ReadMCN

- ReadTOC

- ReadTOC

- ReadTrackInfo

- ReportBlockSize

- ReportEjectability

- ReportKeyDeprecated

- ReportKey

- ReportLockability

- ReportMaxReadTransfer

- ReportMaxValidBlock

- ReportMaxWriteTransfer

- ReportMediaState

- ReportPollRequirements

- ReportRemovability

- ReportWriteProtection

- RequestIdle

- ReserveTrack

- ResetMediaCharacteristics

- ResumeDeviceSupport

- SEND_KEY_V2

- SET_CD_SPEED

- SET_READ_AHEAD

- SET_STREAMING

- START_STOP_UNIT

- SYNCHRONIZE_CACHE

- SendKey

- SetMediaAccessSpeed

- SetMediaCharacteristics

- SetPollingMode

- SetTrayState

- StartDeviceSupport

- StopDeviceSupport

- SuspendDeviceSupport

- SyncReadWrite

- SynchronizeCache

- TerminateDeviceSupport

- TicklePowerManager

- VerifyDeviceState

- WRITE_10

- WRITE_AND_VERIFY_10

- free

- getMetaClass

- setAggressiveness

- setProperties

### Type Methods

+ AsyncReadWriteComplete

+ sPollForMedia

## Relationships

### Inherits From

- IOSCSIPrimaryCommandsDevice

## See Also

### Multimedia Devices

IOSCSILogicalUnitNub

IOSCSIParallelInterfaceController

Class that represents a SCSI Host Bus Adapter.

Deprecated

IOSCSIPeripheralDeviceType05

