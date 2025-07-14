

- Device Management
-  StatusSoftwareUpdateInstallState 

Object

# StatusSoftwareUpdateInstallState

A status report of the software update install state.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object StatusSoftwareUpdateInstallState
```

## Properties

`softwareupdate.install-state`

`string`

 (Required) 

The software update install status, which has the following values:

`none`  
There’s no software update pending, and any previous software update succeeded.

Possible Values: `none, downloading, prepared, installing, failed`

## Overview

`waiting`  
A software update is waiting to start.

`downloading`  
The system is downloading data for a software update.

`prepared`  
The system prepared the software update and it’s ready for installation.

`installing`  
The system is installing the software update.

`failed`  
The software update failed.

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

