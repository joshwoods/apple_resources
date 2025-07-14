

- Kernel
- Hardware Families
- SCSI
-  IOSCSIPrimaryCommandsDevice 

Class

# IOSCSIPrimaryCommandsDevice

macOS 10.6+

``` source
class IOSCSIPrimaryCommandsDevice : IOSCSIProtocolInterface
```

## Topics

### Instance Methods

- AbortCommand

- AbortTask

- AbortTaskSet

- CheckPowerConditionsModePage

- ClampPowerState

- ClearACA

- ClearNotReadyStatus

- ClearPowerOnReset

- ClearTaskSet

- ExecuteCommand

- GatedWaitForTask

- GetANSIVersion

- GetApplicationLayerReference

- GetAutoSenseData

- GetAutoSenseData

- GetAutoSenseDataSize

- GetCMDQUE

- GetDataBuffer

- GetDataTransferDirection

- GetDeviceCharacteristicsDictionary

- GetModeSense

- GetNumberOfPowerStateTransitions

- GetProductString

- GetProtocolCharacteristicsDictionary

- GetProtocolDriver

- GetRealizedDataTransferCount

- GetRequestedDataTransferCount

- GetRetryCount

- GetRevisionString

- GetSCSITask

- GetServiceResponse

- GetTaggedTaskIdentifier

- GetTaskAttribute

- GetTaskState

- GetTaskStatus

- GetTimeoutDuration

- GetUniqueTagID

- GetVendorString

- HandleIncrementOutstandingCommandsCount

- HandleProtocolServiceFeature

- INQUIRY

- INQUIRY

- IncrementOutstandingCommandsCount

- InitializeDeviceSupport

- IsDeviceAccessEnabled

- IsDeviceAccessSuspended

- IsMemoryDescriptorValid

- IsMemoryDescriptorValid

- IsParameterValid

- IsParameterValid

- IsParameterValid

- IsParameterValid

- IsProtocolAccessEnabled

- IsProtocolServiceSupported

- LOG_SELECT

- LOG_SENSE

- LogicalUnitReset

- MODE_SELECT_10

- MODE_SELECT_6

- MODE_SENSE_10

- MODE_SENSE_6

- MapINQUIRYDataToIconFile

- PERSISTENT_RESERVE_IN

- PERSISTENT_RESERVE_OUT

- PREVENT_ALLOW_MEDIUM_REMOVAL

- READ_BUFFER

- RECEIVE

- RECEIVE_DIAGNOSTICS_RESULTS

- RELEASE_10

- RELEASE_6

- REPORT_DEVICE_IDENTIFIER

- REPORT_LUNS

- REQUEST_SENSE

- RESERVE_10

- RESERVE_6

- ReleasePowerStateClamp

- ReleaseSCSITask

- ResetForNewTask

- ResumeDeviceSupport

- RetrieveINQUIRYData

- SEND

- SEND_DIAGNOSTICS

- SET_DEVICE_IDENTIFIER

- SendCommand

- SendCommand

- SetANSIVersion

- SetApplicationLayerReference

- SetAutosenseCommand

- SetCMDQUE

- SetCommandDescriptorBlock

- SetCommandDescriptorBlock

- SetCommandDescriptorBlock

- SetCommandDescriptorBlock

- SetDataBuffer

- SetDataTransferDirection

- SetRealizedDataTransferCount

- SetRequestedDataTransferCount

- SetServiceResponse

- SetTaggedTaskIdentifier

- SetTaskAttribute

- SetTaskCompletionCallback

- SetTaskState

- SetTaskStatus

- SetTimeoutDuration

- StartDeviceSupport

- StopDeviceSupport

- SuspendDeviceSupport

- TEST_UNIT_READY

- TargetReset

- TaskCompletedNotification

- TaskCompletion

- TerminateDeviceSupport

- VerifyDeviceState

- WRITE_BUFFER

- free

- getMetaClass

- init

- message

- setAggressiveness

- start

- stop

### Type Methods

+ ServerKeyswitchCallback

+ TaskCallback

+ sGetOwnerForTask

+ sIncrementOutstandingCommandsCount

+ sWaitForTask

## Relationships

### Inherits From

- IOSCSIProtocolInterface

## See Also

### Base Types

IOReducedBlockServices

IOSCSIPeripheralDeviceNub

IOSCSIProtocolServices

This class defines the public SCSI Protocol Services Layer API for any class that implements SCSI protocol services. A protocol services layer driver is responsible for taking incoming SCSITaskIdentifier objects and translating them to the native command type for the native protocol interface (e.g. SBP-2 ORB on FireWire).

IOSCSIProtocolInterface

This class defines the public SCSI Protocol Layer API for any class that provides Protocol services or needs to provide the Protocol Service API for passing service requests to a Protocol Service driver.

