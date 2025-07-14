

- Device Management
-  StatusSoftwareUpdatePendingVersion 

Object

# StatusSoftwareUpdatePendingVersion

A status report of the pending software update version.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object StatusSoftwareUpdatePendingVersion
```

## Properties

`softwareupdate.pending-version`

StatusSoftwareUpdatePendingVersionDictionaryObject

 (Required) 

A dictionary that contains the build and OS versions of the software update that’s pending on the device.

## Topics

### Supporting Objects

object StatusSoftwareUpdatePendingVersionDictionaryObject

A dictionary that contains details about a pending software update.

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

