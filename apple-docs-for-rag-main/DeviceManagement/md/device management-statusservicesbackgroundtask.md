

- Device Management
-  StatusServicesBackgroundTask 

Object

# StatusServicesBackgroundTask

A status report of the device’s background task details.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object StatusServicesBackgroundTask
```

## Properties

`services.background-task`

`[`StatusServicesBackgroundTaskBackgroundTaskObject`]`

 (Required) 

The background task.

## Topics

### Supporting Objects

object StatusServicesBackgroundTaskBackgroundTaskObject

A status report of a background task.

object StatusServicesBackgroundTaskBackgroundTask_LaunchdObject

A status report of a background task that’s based on a launch daemon.

object StatusServicesBackgroundTaskBackgroundTask_Launchd_DeviceManagementObject

## See Also

### Status Reports and Elements

object StatusReport

A status report of the device’s current state.

object StatusAppManagedList

The device’s declarative managed apps.

object StatusDeviceBatteryHealth

The device’s battery health.

object StatusDeviceModelFamily

A status report of the device’s hardware family.

object StatusDeviceModelIdentifier

A status report of the device’s hardware identifier.

object StatusDeviceModelMarketingName

A status report of the device’s marketing name.

object StatusDeviceModelNumber

A status report of the device’s hardware number.

object StatusDeviceOperatingSystemBuildVersion

A status report of the device’s software build identifier.

object StatusDeviceOperatingSystemFamily

A status report of the device’s operating system family.

object StatusDeviceOperatingSystemSupplementalBuildVersion

A status report of the device’s operating system supplemental build identifier.

object StatusDeviceOperatingSystemSupplementalExtraVersion

A status report of the device’s operating system’s rapid security response identifier.

object StatusDeviceOperatingSystemVersion

A status report of the device’s operating system version.

object StatusDeviceSerialNumber

A status report of the device’s serial number.

object StatusDeviceUDID

A status report of the device’s UDID.

object StatusDiskManagementFileVaultEnabled

The enabled status of the File Vault.

