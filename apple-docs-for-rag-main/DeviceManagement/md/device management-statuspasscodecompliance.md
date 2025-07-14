

- Device Management
-  StatusPasscodeCompliance 

Object

# StatusPasscodeCompliance

A status report of passcode compliance.

iOS 16.0+iPadOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusPasscodeCompliance
```

## Properties

`passcode.is-compliant`

`boolean`

 (Required) 

If `true`, the passcode is in compliance with all passcode policies set on the device. If `false`, the passcode isn’t in compliance with one or more passcode policies set on the device. When there are no passcode policies on the device, this value `true`.

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

